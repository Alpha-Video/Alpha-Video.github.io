---
layout: default
---

## Quick Start
Run this command:
```shell
pip install mvideogallery
```

## Pre-requisites
* [python3](https://www.python.org/)
* [pytorch >= 1.3](https://pytorch.org/)

## Installation
### pip
Run this command:
```shell
pip install mvideogallery
```

### from source
Clone repository from github:
```bash
git clone https://github.com/ mvideogallery
cd mvideogallery
```

Setup and install MVIdeoGallery:
```bash
python setup.py build install
```

## Verification 
Firstly, check the version of MVIdeoGallery.
```python
import mvideogallery
print(mvideogallery.__version__)
```
To ensure that MVIdeoGallery was installed correctly, 
we can verify the installation by running sample MVIdeoGallery code. Here we will construct a MOT model.
```python
model = mvideogallery.model.tubeTK(pretrain=False)
print(model)
```
The output should be something similar to:
```python
...(other structure)...
(TubeTK_cls): Conv3d(256, 1, kernel_size=(3, 3, 3), stride=(1, 1, 1), padding=(1, 1, 1))
    (TubeTK_reg): Conv3d(256, 14, kernel_size=(3, 3, 3), stride=(1, 1, 1), padding=(1, 1, 1))
    (TubeTK_centerness): Conv3d(256, 1, kernel_size=(3, 3, 3), stride=(1, 1, 1), padding=(1, 1, 1))
    (scales): ModuleList(
      (0): Scale()
      (1): Scale()
      (2): Scale()
      (3): Scale()
      (4): Scale()
    )
  )
)

```