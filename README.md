# SplITS

# This repository is under construction
Additional information and instructions to be added.


# Installing SplITS
SplITS is implemented on top of Fuzzware, and follows a similar installation process. We provide the following commands as an example based on Ubuntu 20.04.

```bash
# install dependencies
sudo apt install python2 python3 automake redis-server tmux cmake clang unzip python3-pip
pip3 install virtualenvwrapper
# check the output of pip3 incase commands have to be run to configure the environment

# clone SplITS
git clone https://github.com/SplITS-Fuzzer/SplITS

# get submodules
git submodule update --init --recursive

# compile
cd fuzzware
./install_local.sh
```


# Instructions
SplITS can used using the Fuzzware style commands. AFL++ mode with Split Input To State is enabled by default.

From a folder with an appripriate config file, run the following commands to start a 24 hour fuzzing campaign:

```bash
workon fuzzware
fuzzware pipeline --run-for 24:00:00
```


# Experiments
Information regarding our experiments and results are made available [here.](https://github.com/SplITS-Fuzzer/SplITS-Experiments)

# Found an issue?
If you encounter an issue using SplITS please open an [issue](https://github.com/SplITS-Fuzzer/SplITS/issues).
