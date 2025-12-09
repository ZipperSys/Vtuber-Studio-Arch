# Running VTS on Arch Linux for Vtuber Studio
A little note that the $ is used to indicate the terminal. The distro used is Arch Linux but you can follow this guide with any distro just replace pacman with your provided package manager.

## Requirements
- OpenSeeFace
- Vtuber Studio
- Terminal

## Cloning the OpenSeeFace Github Repo
first clone the OpenSeeFace repo:

```
$ git clone https://github.com/emilianavt/OpenSeeFace
```

## Install Python Dependencies

then make sure you have all the python dependencies needed to use OpenSeeFace (install if needed):

keep in mind that to install packages you need to use sudo.

```
$ pacman -Sy python python-pip python-virtualenv
```
if you already have Python installed then use

```
$ pacman -Sy python python-pip pyhton-virtualenv --needed
```


# Getting into using OpenSeeFace

Once everything is installed start by cding into OpenSeeFace:

```
$ cd OpenSeeFace/
```

then run this command

```
$ virtualenv -p python env
```

this command will then start a Python virtual environment and we will need this to use OpenSeeFace correctly. To start the env run this command :

```
$ source env/bin/activate
```

After starting the env, run this command:

```
$ pip install onnxruntime opencv-python pillow numpy
```

This will 
