## Getting Started (tested for MacOS 15.5)

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

The first time, you need to make the running script usable by 

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

