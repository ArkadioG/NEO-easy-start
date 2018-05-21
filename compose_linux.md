# Installation of docker-compose on Linux

Executed below instructions:

1. download newest version (one line command!)
`sudo curl -L https://github.com/docker/compose/releases/download/1.21.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose`
1. change permissions for docker-compose:  
    `sudo chmod +x /usr/local/bin/docker-compose`
1. check if everything is working:  
    `docker-compose --version`
