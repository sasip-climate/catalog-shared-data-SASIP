# How to access data from GRICAD

 - If you don't have an account, create it [here](https://perseus.univ-grenoble-alpes.fr/create-account/portal) (select chercheur in contract type if you have a permanent position or are a post-doc, doctorant if you are PhD) and ask to join the pr-sasip project.
 - Read carefully the [computation center documentation](https://gricad-doc.univ-grenoble-alpes.fr/en/)
 - Once logged to dahu (CPU) or bigfoot (GPU), you have access to the storage at : ```/summer/sasip```


### Configuration of your access to gricad

You can set up a direct access to dahu via [this procedure](https://gricad-doc.univ-grenoble-alpes.fr/en/hpc/connexion/#connecting-to-the-gateways-without-a-password) so that ssh and scp takes only one line of command, a simplified version is reported below :

  - Check that you should be able to connect to the bastions : ```ssh <your-login>@rotule.u-ga.fr``` and ```ssh <your-login>@trinity.u-ga.fr``` (replace <your-login> with your perseus account)
  - Once connected on one of the bastions, check that you can connect to dahu (for CPU) : ```ssh dahu``` or bigfoot (for GPU) ```ssh bigfoot```
  - To connect directly to dahu or bigfoot, add the following lines to your ```.ssh/config``` :

```bash
Host *
  ServerAliveInterval 30
  AddKeysToAgent yes
  IdentityFile ~/.ssh/id_rsa
  ForwardX11 yes
  TCPKeepAlive yes
 
Host *.ciment
  User <your-login>
  ProxyCommand ssh -q <your-login>@access-gricad.univ-grenoble-alpes.fr "nc -w 60 `basename %h .ciment` %p"
```

  - Now you should be able to connect to dahu directly with ```ssh dahu.ciment``` or to bigfoot with ```ssh bigfoot.ciment```
  - To connect without typing your password, you can set up a SSH key :
    - on your local machine create the ssh key : ```ssh-keygen```
    - copy the public key to the bastions, it is the file in .ssh that ends with .pub, it can be id_rsa.pub or id_ed25519.pub :
    
```ssh-copy-id -i .ssh/KEY.pub <your-login>@rotule.u-ga.fr:``` and  ```ssh-copy-id -i .ssh/KEY.pub <your-login>@trinity.u-ga.fr:``` and to the clusters : ```ssh-copy-id -i .ssh/KEY.pub <your-login>@dahu.ciment:``` or ```ssh-copy-id -i .ssh/KEY.pub <your-login>@bigfoot.ciment:```


## How to share a dataset on the SUMMER storage

Once you connected to dahu, go to ```/summer/sasip```

  - put your data in a repository that has a meaningful name (ex ERAinterim-2012-2020-3h) in the right subdirectory (model-configuration, model-forcing, model-outputs, observations)
  - if needed, change the owner and rights to your directory so that everyone in the pr-sasip group can access it (like ```drwxrwxr-- 4 alberta pr-sasip```for instance)
  - provide a readme file that describes what, who, where, when the data was produced inside the repository (like [this one](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/forcings/ERAinterim-2012-2020-3h.md) for instance)
  - if you are the producer of the dataset, try as much as possible to follow the [FAIR principles](https://cloud.univ-grenoble-alpes.fr/index.php/apps/onlyoffice/s/p4BeQ8mfbniT9oM?fileId=354365064) that SASIP committed to endorse (rich metadata, doi, etc ...)
  - report the same informations on the [catalog on github](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/catalog-details.md) : create a md file in the right subdirectory of github (ex forcings/your-data.md) and make a link to it in forcings.md in this example
  - advertise that your data is available among SASIP participants using participants(at)sasip-climate.com mailing list !

