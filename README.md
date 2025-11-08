## Getting Started (tested for MacOS 15.5)

This repository is a fork of the public version of applio. There are several installation 
options, including the app Dione. I've only managed to install Applio manually on Mac as
follows (probably the same works on Linux). For Windows, refer to the original repo. 

### 1. Installation

Clone this repository with 

```
$ git clone git@github.com:tandradew/Applio_Nova2025.git
```

Create a python environment with python 3.11, for example, using conda, you could do

```
$ conda create -n applio-nova2025 python=3.11
```

Activate the environment with 

```
conda activate applio-nova2025
```

Use the installation script by 

```
$ chmod +x run-install.sh
$ ./run-install.sh
```

You can now deactivate your conda environment, since you will no longer need it

```
conda deactivate 
```

The first time you use applio, you need to make the running script usable by 

```
$ chmod +x run-applio.sh
```


### 2. Running Applio

Start Applio using:

```
$ export PYTORCH_ENABLE_MPS_FALLBACK=1
$ ./run-applio.sh
```

This launches the Gradio interface in your default browser.

The first line is important to avoid calling the gpu which is not
allowed in MacOS, at least for this implementation of Applio. 

### 3. Adding RVC models 

To add RVC voice models, just drag and drop the `.pth` and `.index` files using 
Applio's. You can train them yourself or download them from e.g. 
https://voice-models.com