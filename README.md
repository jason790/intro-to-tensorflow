[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/PythonWorkshop/intro-to-tensorflow)

# Introduction to TensorFlow
In this tutorial the steps needed to clean a dataset and prepare it for modeling using the machine learning library
TensorFlow. The tutorial uses the [Wine](http://archive.ics.uci.edu/ml/datasets/Wine) dataset from the
[UCI Machine Learning Repository](http://archive.ics.uci.edu/ml).

## Prerequisites
This tutorial includes several machine learning terms. To get a good mathematical understanding of these concepts,
please read the [Math Primer](https://github.com/PythonWorkshop/intro-to-tensorflow/blob/master/MathPrimer/Math%20primer%20for%20ML%20%26%20TensorFlow%20workshop.ipynb).

## Installation Notes
There are a few packages you will need in order to run this tutorial. We recommend installing the miniconda environment,
which makes the installation process quite easy. Please see the
[README](https://github.com/PythonWorkshop/intro-to-sklearn) file for this mornings session for instructions on how to
install miniconda.

In order to run this tutorial, you will need the following Python packages:
* numpy 1.11 or later
* pandas 0.18 or later
* matplotlib 1.5 or later
* seaborn 0.7 or later
* scikit-learn 0.17.1 or later
* six 1.10.0 or later
* jupyter
* tensorflow 0.8.0

The first seven packages can be installed with the following command:

```
pip install seaborn scikit-learn jupyter
```

Alternatively if you are using conda you can do:

```
conda install seaborn scikit-learn jupyter
```

For **TensorFlow**, the installation depends on your environment. Below are installation instructions. For detailed
instuctions, please see the TensorFlow
[Download and Setup](https://www.tensorflow.org/versions/r0.8/get_started/os_setup.html#download-and-setup) page.

Note, **skflow** is now part of the TensorFlow library. Once you have installed TensorFlow, you can load skflow with
the following command:

```
import tensorflow.contrib.learn as skflow
```

For detailed instructions about skflow, please read [Skflow Readme](https://github.com/tensorflow/skflow).

### NOTE:
What's better to use? The virtual environment or normal pip installation?

## Playing With Outliers

I have added a fun interactive application using the Python visualization library called Bokeh. The app allows you to
pick features from the wine data set and define an outlier threshold to explore how this affects the data. The
application source code is in the `playing_with_outliers` directory and is called `main.py`. To run this application,
you will need to install bokeh:

```
pip install bokeh
```

Then, to run the application, download the `playing_with_outliers` directory and its contents. Then, in the directory
where you downloaded it, run:

```
bokeh serve --show playing_with_outliers
```

The application will open in your browser.


