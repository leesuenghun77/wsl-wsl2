# wsl-wsl2
wsl wsl2
#!/bin/bash

# Update the package lists
sudo apt-get update

# Upgrade installed packages
sudo apt-get upgrade -y

# Install some useful packages
sudo apt-get install -y \
    git \
    curl \
    build-essential \
    zsh \
    htop \
    tmux \
    vim

# Set up zsh as the default shell
chsh -s /usr/bin/zsh

#!/bin/bash

# Update the package lists
sudo apt-get update

# Upgrade installed packages
sudo apt-get upgrade -y

# Install some useful packages
sudo apt-get install -y \
    git \
    curl \
    build-essential \
    zsh \
    htop \
    tmux \
    vim \
    docker.io \
    docker-compose

# Set up zsh as the default shell
chsh -s /usr/bin/zsh

# Install Docker and Docker Compose
sudo usermod -aG docker $USER
newgrp docker


