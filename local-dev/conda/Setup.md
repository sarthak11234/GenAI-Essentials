## Install Miniconda

https://docs.anaconda.com/miniconda/

```sh
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O /tmp/miniconda.sh
bash /tmp/miniconda.sh -b -u -p ~/miniconda3
```

## Setup Miniconda

```sh
source ~/miniconda3/bin/activate
conda init --all   
```

## Create a new env

Create a new python env called hello, with python version 3.10.0

```sh
conda create --name hello python=3.10.0 -y
```

## Activate the env

```sh
conda activate hello
```

## Get Info about current enviroment

We can see things like where the python envs exists.
```sh
conda info
```

## Remove an env

```sh
conda deactivate
conda remove -n hello --all -y
```