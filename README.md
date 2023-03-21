# Depth Estimation of a Single 2D Image

### Modified From: [High Quality Monocular Depth Estimation via Transfer Learning (arXiv 2018)](https://github.com/ialhashim/DenseDepth)
> **[Ibraheem Alhashim](https://ialhashim.github.io/)** and **Peter Wonka**

## To Run on Windows 10/11

* Download the pretrained model [`nyu.h5`](https://s3-eu-west-1.amazonaws.com/densedepth/nyu.h5) (~165 MB) from the original paper and put in directory
* Download the labeled dataset [`nyu_depth_v2_labeled.mat`](http://horatio.cs.nyu.edu/mit/silberman/nyu_depth_v2/nyu_depth_v2_labeled.mat) (~2.8 GB) and put in directory
* Install python==3.7.9 (the [Windows x86_64 executable installer](https://www.python.org/downloads/release/python-379/) version) (make sure to click add to PATH variable)

* In directory, create virtual environment for packages:
```
$ python -m venv env
$ ./env/Scripts/activate
```
* Install Packages:

```
$ pip install pillow matplotlib scikit-learn scikit-image opencv-python pydot
$ pip install keras==2.2.4
$ pip install tensorflow==1.13.1
$ pip install GraphViz
$ pip install protobuf==3.20
$ pip install 'h5py==2.10.0' --force-reinstall
```
* Open `notebook.ipynb` using the virtual environment kernel and "Run All"
