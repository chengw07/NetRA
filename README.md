# NetRA
Code for "Learning Deep Network Representations with Adversarially Regularized Autoencoders."


NetRA Documentation
---pytorch version
Wei Cheng(weicheng@nec-labs.com)
This is the document of NetRA for pytorch version. For technical details, please refer to the paper:
Learning Deep Network Representations with Adversarially Regularized Autoencoders.
Wenchao Yu, Cheng Zheng, Wei Cheng, Charu Aggarwal, Dongjing Song, Bo Zong, Haifeng Chen, Wei Wang. The Proceedings of the ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (SIGKDD’18), 2018.


The entry of running is ./src/train.py. It conducts embedding of nodes in a static network (karate network) and visualizes the 2-dimensional embedding results of nodes. The html docs for each python file are included in ./doc_html. To better understand the framework, the reader is supposed to be familiar with pytorch framework and Wasserstein GAN.


System Requirements

We need python 2.7 and torch 0.3.1.

1). Install using the Homebrew package manager:

Mac:

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
export PATH="/usr/local/bin:/usr/local/sbin:$PATH"
brew update
brew install python@2  # Python 2
sudo pip install -U virtualenv  # system-wide install

Ubuntu:

sudo apt update
sudo apt install python-dev python-pip
sudo pip install -U virtualenv  # system-wide install

2). Create a new virtual environment by choosing a Python interpreter


virtualenv --system-site-packages -p python2.7 ./venv
source ./venv/bin/activate
pip install --upgrade pip

3). install torch version 0.3.1
pip install torch==0.3.1


4). install packages
pip install networkx
pip install scipy
