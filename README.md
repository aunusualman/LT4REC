
This is the code implementation of LT4REC.
We demonstrate the algorithm on the dataset gathered from traffic
logs of real world video recommendation system.
## Enviroments

tensorflow==1.12

tensorboard==1.12

pyyaml

absl-py

numpy

sklearn

## Installation

```bash
pip3 install -r requirements.txt
```

## Dataset

For the dataset gathered from traffic logs of real world video recommendation system 
is not completely public, we just provide a small part of the dataset. Download the dataset demo from .... The data is stored as the tfrecord format, with feature columns defined as:
```
features{
 FEA_SVID: {tf.FixedLenFeature([], tf.string)}
    FEA_SCP: {tf.FixedLenFeature([], tf.string)}          
    FEA_SICAT1: {tf.FixedLenFeature([], tf.string)}         
    FEA_SICAT2: {tf.FixedLenFeature([], tf.string)}          
    FEA_SIKEYWORD: {tf.FixedLenSequenceFeature([], tf.string)}  
    FEA_STAG: {tf.FixedLenSequenceFeature([], tf.string)}
    FEA_VID: {tf.FixedLenFeature([], tf.string)}    
    FEA_CP: {tf.FixedLenFeature([], tf.string)}   
    FEA_ICAT1: {tf.FixedLenFeature([], tf.string)}   
    FEA_ICAT2: {tf.FixedLenFeature([], tf.string)}   
    FEA_IXFTAG: {tf.FixedLenSequenceFeature([], tf.string)}
    ...
    playrate: {tf.FixedLenFeature([], tf.float32)} 
    label: {tf.FixedLenFeature([], tf.int64)} 
    }
```

