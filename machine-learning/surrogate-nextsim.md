# Repository surrogate_nextsim

This repository [(here)](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/machine-learning-data/surrogate_nextsim/catalog.html) contains data to train and test a data-driven surrogate model for neXtSIM

In folder **source_files**, original data for 2009 are available for plot purposes

In folder **SIT_data_tfrecords** is posted the ready-to-train dataset in tfrecords style [(doc)](https://www.tensorflow.org/tutorials/load_data/tfrecord?hl=en#tfrecords_format_details)

The goal is to train a UNet-based neural network to learn the dynamic of the sea-ice thickness in a smaller resolution than original data (~40km resolution). 

**contact : charlotte.durand(at)enpc.fr**
