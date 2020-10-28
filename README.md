# Openvino Course

Openvino course lectured at UFRN/Natal on summer 2020

## Prerequisites
* Git - [Download & Install Git](https://git-scm.com/downloads). OSX and Linux machines typically have this already installed.
* Pip - [Or prefered python package manager](https://pip.pypa.io/en/stable/installing/).
* Python 3.6+ - [Recomended Instalation through pyenv](https://www.python.org/).
* OpenVino 2021.1 - [Latest version at time of writing](https://docs.openvinotoolkit.org/2021.1/openvino_docs_get_started_get_started_linux.html).

# Example usage

## Model optimizer

### Activate virtual enviroment

```
source /opt/intel/openvino_2021.1.110/deployment_tools/model_optimizer/install_prerequisites/../venv/bin/activate

```

### Convert Model
```

python3 /opt/intel/openvino_2021/deployment_tools/model_optimizer/mo_tf.py --saved_model_dir Examples/Transfer_learning/pretrained_model/ --input_shape [1,160,160,3] --output_dir fp_16 --progress

```