# gpu_tpu_lab_server
> Running a jupyter lab or vs code server environment from colab with google drive support.<br><br>


## Motivation for creating this package
1. For some reason in [fns](https://github.com/amitness/fns/) python package version >=0.5, fns.colab supports only normal jupyter notebook with drive support, so here I have used the previous version of that fns.colab code to support jupyter lab environment.
1. It was boring to copy paste the whole code everytime to start the jupyter lab environment in colab, so I created a package of it. 
1. Also, I wanted to try how to create python package using nbdev, this sounded like a good excuse.


## Install

`pip install gpu_tpu_lab_server`

## How to use

```
from gpu_tpu_lab_server.core import jupyter_lab, vscode, run_process_in_background, run_process_in_foreground
```

## For starting the server in google colab with google_drive support
### To enable jupyter_lab_environment
1. execute `jupyter_lab()`  
2. an authorization window will open with a link, go to the link > select your google account > accept all the permissions > authorization code will be displayed > copy and paste the code in the window
3. an localtunnel link will be returned, go to that link, wait for 10 second, then press open tunnel button, it will open an jupyter lab environment

### To enable vscode() environment
1. execute `vscode()` optional parameter any text :- the generated link will have the text or by default fastdaima
2. an authorization window will open with a link, go to the link > select your google account > accept all the permissions > authorization code will be displayed > copy and paste the code in the window
3. an localtunnel link will be returned, go to that link it will open an vscode server environment
