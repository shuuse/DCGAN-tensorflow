# Code used for my SCI52 assignment


## Prerequisites

- Python 3.6+
- [Tensorflow 0.12.1](https://github.com/tensorflow/tensorflow/tree/r0.12)
- [SciPy](http://www.scipy.org/install.html)
- [pillow](https://github.com/python-pillow/Pillow)
- opencv

## Usage

First, download dataset with:

    $ python download.py mnist celebA

To train a model with downloaded dataset:

    $ python main.py --dataset celebA --input_height=108 --train --crop --out_name="mytrainingfolder"

To test with an existing model:

    $ python main.py --dataset celebA --input_height=108 --crop --visualize true --out_name="mytrainingfolder"


## Online Demo (Taehoon Kim's page)

[<img src="https://raw.githubusercontent.com/carpedm20/blog/master/content/images/face.png">](http://carpedm20.github.io/faces/)

[link](http://carpedm20.github.io/faces/)



## Author

Taehoon Kim / [@carpedm20](http://carpedm20.github.io/)
