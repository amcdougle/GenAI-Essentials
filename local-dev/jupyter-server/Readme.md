#Install Miniconda

https://www.anaconda.com/docs/getting-started/miniconda/main

'''sh
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O /tmp/miniconda.sh
bash /tmp/miniconda.sh -b -u -p ~/miniconda3
'''
## setup minconda
'''sh
source ~/miniconda3/bin/activate
conda init --all    
'''

#create a new env 
'''sh
conda create --name openvino python=3.10.0 -y
'''

## Activate the env 
'''sh
conda activate openvino
'''


## Get info about current env 
'''sh
conda info
'''

## deactivate env

''sh
conda deactivate
'''

## remove from env
'''sh
conda remove -n openvino --all -y
'''

```sh
conda create -n serv python=3.10.0 ipykernel -y
conda install -c conda-forge jupyterlab
jupyter lab --no-browser --allow-root --ip 0.0.0.0
conda install -c conda-forge jupyterlab-git
conda install -c conda-forge catppuccin-jupyterlab
```
