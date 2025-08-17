# compile-python
This is a repo for compiling and installing python from scratch

## Compile python and creating a virtualEnv with it
$ sudo apt-get install build-essential gdb lcov libbz2-dev libffi-dev libgdbm-dev liblzma-dev libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev lzma lzma-dev tk-dev uuid-dev zlib1g-dev

# downloading python version
$ wget https://www.python.org/ftp/python/3.12.11/Python-3.12.11.tgz

# unzipping python .tgz file
$ tar zxvf Python-3.12.11.tgz

# Configuring python virtualEnv 
$ cd Python-3.12.11
$ ./configure --enable-optimizations

# installing Packages
$ make -j 16
$ make altinstall
$ sudo make altinstall
$ /usr/local/bin/python3.12
$ vim ~/.bashrc
# new python env path
alias python="/usr/local/bin/python3.12"
$ source ~/.bashrc
$ python

$ python -m venv ~/.venv
$ vim ~/.bashrc
# source venv
source ~/.venv/bin/activate
$ source ~/.bashrc
$ which python
/home/codespace/.venv/bin/python

$ make install
$ git status

$ git status
$ git add
$ git commit -m "adding skeleton"
$ git push

$ rm -rf Python-3.12.11/
$ git restore --staged Python-3.12.11/