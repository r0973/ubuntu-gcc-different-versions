# ubuntu-gcc-different-versions
how to install different versions of gcc, g++, gfortran on ubuntu

sudo apt-get update -y && <br/>
sudo apt-get upgrade -y && <br/>
sudo apt-get install build-essential software-properties-common -y && <br/>
sudo add-apt-repository ppa:ubuntu-toolchain-r/test -y && <br/>
sudo apt-get update -y && <br/>
sudo apt-get install gcc-9 g++-9 gfortran-9 -y && <br/>
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 60 \ <br/>
--slave /usr/bin/g++ g++ /usr/bin/g++-9 \ <br/>
--slave /usr/bin/gfortran gfortran /usr/bin/gfortran-9 <br/>
sudo update-alternatives --config gcc
