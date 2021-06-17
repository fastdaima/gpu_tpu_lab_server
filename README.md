# gpu_tpu_lab_server
> Running a jupyter lab or vs code server environment from colab with google drive support.<br><br>


## Motivation for creating this package
1. For some reason in [fns](https://github.com/amitness/fns/) python package version >=0.5, fns.colab supports only normal jupyter notebook with drive support, so here I have used the previous version of that fns.colab code to support jupyter lab environment.
1. It was boring to copy paste the whole code everytime to start the jupyter lab environment in colab, so I created a package of it. 
1. Also, I wanted to try how to create python package using nbdev, this sounded like a good excuse.


## Install

`pip install gpu_tpu_lab_server`

## How to use

```python
from gpu_tpu_lab_server.core import jupyter_lab
```

### run
jupyter_lab()  # for jupyter_lab environment <br>
vscode()  # for vscode server environment
