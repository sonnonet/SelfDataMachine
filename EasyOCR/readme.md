# EasyOCR


# Test Enviroment
  - Rasberrypi OS (rasibian)
  - python Version 3.9.2
  - 
## Error
```
Python 3.9.2 (default, Feb 28 2021, 17:03:44) 
[GCC 10.2.1 20210110] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import easyocr
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/home/pi/.local/lib/python3.9/site-packages/easyocr/__init__.py", line 1, in <module>
    from .easyocr import Reader
  File "/home/pi/.local/lib/python3.9/site-packages/easyocr/easyocr.py", line 3, in <module>
    from .recognition import get_recognizer, get_text
  File "/home/pi/.local/lib/python3.9/site-packages/easyocr/recognition.py", line 2, in <module>
    import torch
  File "/home/pi/.local/lib/python3.9/site-packages/torch/__init__.py", line 1429, in <module>
    from torch import optim as optim
  File "/home/pi/.local/lib/python3.9/site-packages/torch/optim/__init__.py", line 8, in <module>
    from .adadelta import Adadelta
  File "/home/pi/.local/lib/python3.9/site-packages/torch/optim/adadelta.py", line 4, in <module>
    from .optimizer import (Optimizer, _use_grad_for_differentiable, _default_to_fused_or_foreach,
  File "/home/pi/.local/lib/python3.9/site-packages/torch/optim/optimizer.py", line 23, in <module>
    from typing_extensions import ParamSpec, Self, TypeAlias
ImportError: cannot import name 'ParamSpec' from 'typing_extensions' (/usr/lib/python3/dist-packages/typing_extensions.py)

```
  - typing-extencsions Version check
  - solved
  ```
   pip install typing-extension==4.2
  ```
