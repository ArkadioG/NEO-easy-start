# Installing neo-local

**neo-local** it's the easiest way to install:
* **privnet** - private blockchain
* **neo-python** - development CLI
* **neo-scan** - block explorer
* postgre - db for neo-scan

## Download, installation and running neo-local

**Windows - details: [click here](neo-local-win.md)**

1. clone repository **neo-local** to some folder:  
    `git clone https://github.com/neoauth/neo-local.git`

1. cd into neo-local repository:  
    `cd /neo-local`
    
1. run command:  
    `make start`  
    It will take a while to download and run all containers. After installation finishes, automatically will launch **neo-python** CLI and your console window will look similar to that:  
    ![neo-scan instalacja](https://user-images.githubusercontent.com/2796074/36632958-9247f8ba-198d-11e8-8055-f096141902d9.png)
    
 1. To exit neo-python console write command `exit`
 
 1. To stop whole network, within terminal run command `make stop`
 
 #### [Next step - openning wallet](wallet.md) 