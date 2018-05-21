# NEO Smart Contracts with Python Quick Start

## Opis warsztatu

Blockchain to ostatnio bardzo modne pojęcie ze względu na krociowe zyski, które można było odnieść zakupując kryptowaluty.
W części teoretycznej warsztatu poznasz pojęcia związane z blockchainem, zasadę jego działania oraz dowiesz się na jakiej zasadzie działają inteligentne kontrakty* (smart contract). W części warsztatowej napiszemy własny smart contract, który wdrożymy w prywatnym blockchainie NEO.

\* *inteligentny kontrakt najprościej wytłumaczyć jako zwykły progam, który wykonuje zadania w zależności od inputu (**jeśli A to zrób B**), w połączeniu z cechami jakimi charakteryzuje się blockchain, inteligentny kontrakt stwarza niezwykłe możliwości do automatyzowania zadań, które obecnie wymagają zaufanego pośrednika (notariusza, banku itp.).*

## Prerequisites


* Operating system: Win*/**Linux**/OSx  
    Linux is preferred
    
* Install **Python 3.6**:  
  <https://www.python.org/downloads/>
    
  * Windows - details [here](python_win.md)
  * Linux - details [here](python_unix.md)

* Install and run **Docker**:
  
  * Windows: <https://docs.docker.com/docker-for-windows/install/>  
  **CAREFUL** you need HyperV to install docker
  * Ubuntu/Debian/Fedora: <https://docs.docker.com/install/linux/docker-ce/ubuntu/>
  * Linux Mint: details [here](docker_mint.md)
  * Mac: <https://docs.docker.com/docker-for-mac/install/>

* Install **Docker Compose**
    * Win/Mac: already installed with docker
    * Linux: details [here](compose_linux.md)

* check if docker is running <https://docs.docker.com/get-started/#test-docker-installation>

  * run command: `docker --version`
  * additionally, you can run test container `docker run hello-world`
  * listing images: `docker image ls`
  * listing containers: `docker container ls -a`
  
* Install any IDE to work with Python:
    * [PyCharm](https://www.jetbrains.com/toolbox/app/?fromMenu)
    * [Visual Studio Code](https://code.visualstudio.com/)
    * anything else
    
#### [Next Step - installing private blockchain NEO](neo-local.md) 
