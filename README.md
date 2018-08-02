# INSTALAÇÃO CLASSIFICADOR CAFFE - Ubuntu 16.04

> sudo apt-get update
> sudo apt-get upgrade
> sudo apt-get install -y build-essential cmake git pkg-config
> sudo apt-get install -y libprotobuf-dev libleveldb-dev libsnappy-dev libhdf5-serial-dev protobuf-compiler
> sudo apt-get install -y libatlas-base-dev 
> sudo apt-get install -y --no-install-recommends libboost-all-dev
> sudo apt-get install -y libgflags-dev libgoogle-glog-dev liblmdb-dev
> sudo apt-get install -y python3-dev
> sudo apt-get install -y python3-numpy python3-scipy

Download: https://github.com/BVLC/caffe

> cd caffe-master
> cp Makefile.config.example Makefile.config

	* Se for usar o classificador Caffe apenas com uso do CPU, 

	* retire o comentário na linha: CPU_ONLY := 1 no Makefile.config.

 
> mkdir build
> cd build
> cmake ..
> make all
> make install
> make runtest
