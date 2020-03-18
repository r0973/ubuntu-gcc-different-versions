# ubuntu-gcc-different-versions
how to install different versions of gcc, g++, gfortran on ubuntu

sudo apt-get update -y && 
sudo apt-get upgrade -y && 
sudo apt-get install build-essential software-properties-common -y && 
sudo add-apt-repository ppa:ubuntu-toolchain-r/test -y && 
sudo apt-get update -y && 
sudo apt-get install gcc-9 g++-9 gfortran-9 -y && 
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 60 --slave /usr/bin/g++ g++ /usr/bin/g++-9 --slave /usr/bin/gfortran gfortran /usr/bin/gfortran-9
sudo update-alternatives --config gcc
