# NEO beIT

Materiały z prezentacji na konferencji beIT

## Opis warsztatu

Blockchain to ostatnio bardzo modne pojęcie ze względu na krociowe zyski, które można było odnieść zakupując kryptowaluty.
W części teoretycznej warsztatu poznasz pojęcia związane z blockchainem, zasadę jego działania oraz dowiesz się na jakiej zasadzie działają inteligentne kontrakty* (smart contract). W części warsztatowej napiszemy własny smart contract, który wdrożymy w prywatnym blockchainie NEO.

\* *inteligentny kontrakt najprościej wytłumaczyć jako zwykły progam, który wykonuje zadania w zależności od inputu (**jeśli A to zrób B**), w połączeniu z cechami jakimi charakteryzuje się blockchain, inteligentny kontrakt stwarza niezwykłe możliwości do automatyzowania zadań, które obecnie wymagają zaufanego pośrednika (notariusza, banku itp.).*

## Przygotowanie do warsztatu

### Aktualizacja: ***21-04-2018 23:15***

**Sprawdź na kilka dni przed warsztatem czy kroki dotyczące instalacji nie zostały zaktualizowane. W razie problemów z instalacją/przygotowaniem privnetu możesz zgłosić buga używając opcji w github.**


* Wymagany system: Win*/**Linux**/OSx  
    preferowany jest Linux - jeśli używasz innego systemu to zainstaluj Linuxa w maszynie wirtualnej
    
* Zainstaluj **Python 3.6**:  
  <https://www.python.org/downloads/>
    
  * Windows - zobacz szczegóły [tutaj](python_win.md)
  * Linux - zobacz szczegóły [tutaj](python_unix.md)

* Zainstaluj i uruchom **Docker**:
  
  * Windows: <https://docs.docker.com/docker-for-windows/install/>  
  **UWAGA** musisz mieć zainstalowany HyperV, aby zainstalować Docker'a
  * Ubuntu/Debian/Fedora: <https://docs.docker.com/install/linux/docker-ce/ubuntu/>
  * Mint: szczegóły [tutaj](docker_mint.md)
  * Mac: <https://docs.docker.com/docker-for-mac/install/>

* zainstaluj **Docker Compose**
    * Win: już zainstalowane razem z Dockerem
    * Linux: szczegóły [tutaj](compose_linux.md)

* sprawdź czy docker jest uruchomiony <https://docs.docker.com/get-started/#test-docker-installation>

  * wpisz w terminalu/wierszu poleceń komendę: `docker --version`
  * możesz dodatkowo zainstalować testowy kontener:  
    wpisz komendę `docker run hello-world` - docker pobierze, zainstaluje i uruchomi testowy obraz
  * możesz wylistować obrazy: `docker image ls`
  * możesz wylistować kontenery: `docker container ls -a`
  
* Zainstaluj sobie dowolne IDE do pracy z Pythonem:
    * [PyCharm](https://www.jetbrains.com/toolbox/app/?fromMenu)
    * [Visual Studio Code](https://code.visualstudio.com/)
    * coś innego
    
#### [Kolejny krok - instalacja blockchain NEO](neo-local.md) 

## Slajdy

Slajdy pdf z warsztatu dostępne są [tutaj](slajdy.pdf)