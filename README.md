# vs-code-experiment
Experiment of various vs code features

## Git in WSL

git config --global user.name "Xiao Cheng"

git config --global user.email "shane85cheng@gmail.com"

## Line Ending

.gitattributes

## Docker 

install Docker Desktop 

## Validate GPU in wsl2

docker run --rm -it --gpus=all nvcr.io/nvidia/k8s/cuda-sample:nbody nbody -gpu -benchmark

## Vs code developer in containter
git clone source code
Remote-container: open folder in container. 

## Linux X11 app

windows build 22000 version at least

wsl gpu driver

wsl2 is required

## WSL2 kernel update
wsl --update

## CUDA in wsl2

 distribution=$(. /etc/os-release;echo $ID$VERSION_ID)

 install nvidia-docker2

 building cuda in wsl2

 install cuda in wsl2



 wget https://developer.download.nvidia.com/compute/cuda/repos/wsl-ubuntu/x86_64/cuda-wsl-ubuntu.pin

sudo mv cuda-wsl-ubuntu.pin /etc/apt/preferences.d/cuda-repository-pin-600

wget https://developer.download.nvidia.com/compute/cuda/11.4.0/local_installers/cuda-repo-wsl-ubuntu-11-4-local_11.4.0-1_amd64.deb

sudo dpkg -i cuda-repo-wsl-ubuntu-11-6-local_11.6.0-1_amd64.deb

sudo apt-key add /var/cuda-repo-wsl-ubuntu-11-6-local/7fa2af80.pub

sudo apt-get update

sudo apt-get -y install cuda

cd /usr/local/cuda-11.4/samples/4_Finance/BlackScholes

make BlackScholes


# C++ in wsl2

