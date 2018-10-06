# Install tensorflow with anaconda
### February 18, 2018
1. Go to https://www.anaconda.com/download to download anaconda  
2. open terminal and change directoray to where anaconda.sh is, then bash it.  
> bash Anaconda3-5.1.0-Linux-x86_64.sh
3. build anaconda environment named tensorflow
> conda create --name tensorflow python=3
4. active tensorflow environment
> source activate tensorflow
5. install tensorflow
> pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-1.5.0-cp36-cp36m-linux_x86_64.whl
6. To open Anaconda Navigator
> anaconda-navigator
7. install jupyter notebook in home window
8. import environment-cpu.yml to Anaconda
9. hit Environments in left column, run tf-cpu with jupyter notebook

# attachment:
### environmnet-cpu.yml
```
name: tf-cpu
channels:
    - https://conda.anaconda.org/menpo
    - conda-forge
dependencies:
    - python==3.5.2
    - numpy
    - matplotlib
    - jupyter
    - opencv3
    - pillow
    - scikit-learn
    - scikit-image
    - scipy
    - h5py
    - eventlet
    - flask-socketio
    - seaborn
    - pandas
    - ffmpeg
    - imageio=2.1.2
    - pyqt=4.11.4
    - pip:
        - moviepy
        - tensorflow==1.4.0
        - keras==2.0.8
```
