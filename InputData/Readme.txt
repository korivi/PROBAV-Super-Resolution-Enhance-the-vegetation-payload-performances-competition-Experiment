Data Source Link: https://kelvins.esa.int/proba-v-super-resolution/data/

The data for this competition can be downloaded as a compressed zip file (675MB).

Contents:

The zip file is organized as follows:

train/NIR images from the NIR channel of PROBA-V for training
train/RED images from the RED channel of PROBA-V for training
test/NIR images from the NIR channel of PROBA-V to produce the submission
test/RED images from the RED channel of PROBA-V to produce the submission
norm.csv cPSNR of a baseline solution which is used to normalize the submissions (see scoring)
Each scene is saved in a separate folder, named imgsetxxxx, where xxxx is a running number from 0000 to 1449. Each scene in the training folders contains the following file:

HR.png: high resolution image (ground truth for super-resolution)
SM.png: status map of HR.png, indicating clear pixels by a value of 1
LRXXX.png: low resolution image
QMXXX.png: status map of LRXXX.png, indicating clear pixels by a value of 1
The scenes in the test folders are structured the same, but do not include HR.png as your task is to reconstruct it! They include however SM.png, so you know which pixels do count.

