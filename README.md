# SIOS workshop
Hands on workshop on sea ice surface AI classification techniques (<a href="AI4Svalbard workshop (September 2022)">AI4Svalbard</a>, Sep 2022)

<img src="preview/OLCI_SAR.jpg" height="300"/>
<img src="preview/SAR_index.jpg" height="300"/>

Tool for manual image segmentation and classification of satellite imagery (or images in general). It was designed to accelerate the creation of machine learning training datasets for Earth Observation. This application is a flask app which can be run locally. Special highlights:
* Support by AI (gradient boosted decision tree) when doing image segmentation
* Multiple and configurable views for multispectral imagery
* Simple setup with pip and one configuration file
* Platform independent app (runs on Linux, Windows and Mac OS)
* Multi-user support: work in a team on your dataset and merge the results

## Installation

Clone the repository, navigate to the directory, and install the package and its dependencies

```
git clone git@github.com:ESA-PhiLab/iris.git
cd iris
python setup.py install
```

If you are altering the IRIS source code then you made find it easier to install like below, to avoid having to reinstall it every time a change is made
```
pip install -e ./
```

## Usage

Once installed, you can run the demo version of IRIS

```
iris demo
```

Having run the demo, you can then create a personalised config file, based on _demo/cloud-segmentation.json_. With your own config file, you can then instantiate your own custom project

```
iris label <your-config-file>
```

**Visit the official iris Github page:  https://github.com/ESA-PhiLab/iris**
