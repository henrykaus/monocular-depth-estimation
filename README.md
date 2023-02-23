# Monocular Depth Estimation

### Modified From: High Quality Monocular Depth Estimation via Transfer Learning (arXiv 2018)
> **[Ibraheem Alhashim](https://ialhashim.github.io/)** and **Peter Wonka**

## To Run on Windows 10/11

* Download the pretrained model from the original paper [NYU Depth V2](https://s3-eu-west-1.amazonaws.com/densedepth/nyu.h5) (165 MB) and put in directory

* Install python==3.7.9 (the [x86_64 version](https://www.python.org/downloads/release/python-379/)) (make sure to click add to PATH variable)


* Create virtual environment for packages:
```
$ python -m venv env
$ ./env/Scripts/activate
```
* Install Packages:

```$ pip install pillow matplotlib scikit-learn scikit-image opencv-python pydot
$ pip install kera==2.2.4
$ pip install tensorflow==1.13.1
$ pip install GraphViz
$ pip install protobuf==3.20
$ pip install 'h5py==2.10.0' --force-reinstall
```
* In virtual environment on the command line, run the command: `python test.py --model .\nyu.h5`.
This will create heatmaps of images from `/my_examples` into a single `results.png`. This takes approx. 20-60 seconds.

## Reference
Corresponding paper to cite:
```
@article{Alhashim2018,
  author    = {Ibraheem Alhashim and Peter Wonka},
  title     = {High Quality Monocular Depth Estimation via Transfer Learning},
  journal   = {arXiv e-prints},
  volume    = {abs/1812.11941},
  year      = {2018},
  url       = {https://arxiv.org/abs/1812.11941},
  eid       = {arXiv:1812.11941},
  eprint    = {1812.11941}
}
```
