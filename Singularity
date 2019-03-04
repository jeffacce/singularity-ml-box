Bootstrap: docker
From: nvidia/cuda:10.0-cudnn7-devel-ubuntu18.04

%post
        apt-get update
        apt-get install -y tmux vim wget curl
        apt-get install -y python3.6 python3.6-dev python3.6-distutils
        apt-get install -y libglib2.0-0
        curl https://bootstrap.pypa.io/get-pip.py | python3.6
        pip3.6 --no-cache-dir install --upgrade pip
        pip3.6 --no-cache-dir install https://download.pytorch.org/whl/cu100/torch-1.0.1.post2-cp36-cp36m-linux_x86_64.whl
        pip3.6 --no-cache-dir install torchvision
        pip3.6 --no-cache-dir install h5py graphviz pydot
        pip3.6 --no-cache-dir install scipy numpy matplotlib scikit-learn pandas opencv-python
        pip3.6 --no-cache-dir install ipdb imgaug jupyter notebook ipython jupyterlab
        pip3.6 --no-cache-dir install tensorflow-gpu
        pip3.6 --no-cache-dir install Keras
        pip3.6 --no-cache-dir install virtualenv tqdm seaborn requests
        pip3.6 --no-cache-dir install 'tornado>=4, <6'
