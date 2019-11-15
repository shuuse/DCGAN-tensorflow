# DCGAN - Face generation

## Prerequisites

- Python 3.6+
- [Tensorflow 0.12.1](https://github.com/tensorflow/tensorflow/tree/r0.12)
- [SciPy](http://www.scipy.org/install.html)
- [pillow](https://github.com/python-pillow/Pillow)
- opencv

## Download dataset:

First, download dataset with:

    $ python download.py mnist celebA

## Training:
To train a model with downloaded dataset:

    $ python main.py --dataset celebA --input_height=108 --train --crop --out_name='mytrainingfolder'

## Test the results:
To test the results with a trained model:

    $ python main.py --dataset celebA --input_height=108 --crop --visualize true --out_name='mytrainingfolder'

This will start to generate image files in the sample directory under your training folder. Stop the code, and check out the files.

## Alterations: 

### Learning rate:
To change the learning rate, replacing the learning rate with your chosen value:
 $ python main.py --learning_rate='0.0002' --dataset celebA --input_height=108 --train --crop  --out_name='mytrainingfolder'
 
### Double generator update: 
To remove the alteration added by Kim, comment out lines 288-290 in the file "model.py" and run the training again.

## Original code author

Taehoon Kim / [@carpedm20](http://carpedm20.github.io/)
