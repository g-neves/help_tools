#!/usr/bin/env bash

# How to install nvim on Amazon EC2
# CODE FROM https://gist.github.com/kawaz/393c7f62fe6e857cc3d9
sudo yum groups install -y Development\ tools
sudo yum install -y cmake
sudo yum install -y python34-{devel,pip}
sudo pip-3.4 install neovim --upgrade
(
cd "$(mktemp -d)"
git clone https://github.com/neovim/neovim.git
cd neovim
make CMAKE_BUILD_TYPE=Release
sudo make install
)
