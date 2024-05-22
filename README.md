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

#!/bin/bash

# 원본 가상 머신 파일 경로
original_vm="/path/to/original.vmdk"

# 복제할 가상 머신 파일 경로
cloned_vm="/path/to/cloned.vmdk"

# APFS 클로닝 실행
sudo /usr/sbin/asr -source "$original_vm" -target "$cloned_vm"

echo "APFS 클로닝이 완료되었습니다!"

