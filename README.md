# Handwritten Letter Recognition

## Description

- This is a project done at University of Florida under the course Foundations of Machine Learning at Fall 2018 . 
- The program made was a handwritten letter recognition with a scope of letters a,b,c,d,h,i,j,k
- The members were: Joshua Siy, Ezequiel Garcia, Gayatri Behera and Junghoon Woo.  


## Script Descriptions

- `train.py` - Train and cross validate a CNN to classify handwritten characters.

- `test.py` - Test pre-trained CNN.

## Running code

**Important Information**: The code was written in python 3.6.7 using PyTorch
library version 0.4.1.

To classify the 'a and b/easy' dataset, run:

```
python test.py abData.npy out
```

where `abData.npy` can be a different name.

To classify the 'hard' dataset with 8 letters and unknowns, specify the `-e` flag:

```
python test.py hardData.npy out -e
```

where `hardData.npy` can be a different name.

To verify that our `train.py` script works, simply run:

```
python train.py
```

This uses the training data set we last trained the CNN on. The script may take
a while to run since it will run for at least 150 epochs. **IMPORTANT** The
script will overwrite files when it executes.

## Libraries Used

The list of libraries used is

- copy
- json
- matplotlib
- numpy
- os
- pytorch
- torchvision
- scikit-image
- scikit-learn
- scipy
- sys

## CNN Struture

The parameters of the CNN are

- conv1.weight
- conv1.bias
- conv2.weight
- conv2.bias
- fc1.weight
- fc1.bias
- fc2.weight
- fc2.bias

Notice that learning rate and momentum are not included.
