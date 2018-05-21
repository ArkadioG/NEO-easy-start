# Installing Python 3.6 on Linux Ubuntu/Mint

With most probability your main Python3 version will be 3.5.2. We need Python 3.6. Execute below instructions:

1. check if you have Python 3.6 on your system
    * launch command `python3 -V`
        - if answer is not `Python 3.6.x` go to next step
        - if answer is `Python 3.6.x` then further in tutorial use `python3`
    * run command `python3.6` 
        - if command is not recognized, you have to install Python 3.6
        - if Python interpreter launch - further in tutorial use `python3.6` 
    
1. installing Python 3.6
    * add repository with Python 3.6 to sysytem: `sudo add-apt-repository ppa:jonathonf/python-3.6`
    * update apt: `sudo apt-get update`
    * install Python 3.6: `sudo apt-get install python3.6`
    * check correctness of installation: `python3.6 -V` you should see in response `Python 3.6.3`
    * further in workshop use command `python3.6`
    
     
      