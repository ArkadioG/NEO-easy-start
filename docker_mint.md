# Docker installation on Linux Mint 18.3

Official documentation on docker site has mistakes, below steps will wnsure docker will be installed properly on your Linux Mint machine. Additionaly you won't be needing to call `sudo` everytime using docker.

1. execute below commands:
    ```bash
    # import PGP key
     
    sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 \
    --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
     
    # add official repository to package manager 
     
    sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-xenial main'
     
    # update packages
     
    sudo apt update
    
    # install dependencies
     
    sudo apt install linux-image-generic linux-image-extra-virtual
     
    # Reboot
     
    sudo reboot
    
    # Install Docker
     
    sudo apt install docker-engine
    
    ```

1. Change settings to use docker without `sudo`  
    <https://docs.docker.com/install/linux/linux-postinstall/#manage-docker-as-a-non-root-user>
    ```bash
    sudo groupadd docker
    sudo usermod -aG docker $USER
    ```
    
    Now you should be able to use docker without `sudo`. Run example to check correctness of installation: `docker run hello-world`