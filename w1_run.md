# Warsztat

**Jeśli uruchomiłeś kontener bez zmapowanego folderu, w którym będziemy zapisywać kod kontraktów, to musisz:**
* usunąć kontener:
    `docker container rm -f neo-privnet-with-gas`
* utworzyć folder dla kontraktów na swojej maszynie i uruchomić kontener ze zmapowanym folderem - [instrukcje znajdują się w pliku README.md](README.md)

## Uruchomienie privneta

Jeśli zamknąłeś privnet lub docker musisz go ponownie uruchomić.

* Sprawdź czy kontener **neo-privnet-with-gas** jest uruchomiony, wpisz polecenie   
`docker container ls -a`  
flaga `-a` pokaże wszystkie kontenery, również zatrzymane.

> **Podpowiedź**
>
> Zamiast pełnej nazwy kontenera `neo-privnet-with-gas` możesz podawać kilka pierwszych znaków id kontenera - weźmiesz je z pierwszej kolumny po wylistowaniu poleceniem `docker container ls -a`.

* Jeśli jest zatrzymany uruchom go ponownie:  
`docker container start neo-privnet-with-gas`

* Wejdź do terminala wewnątrz kontenera:  
`docker exec -it neo-privnet-with-gas /bin/bash`

W tym momencie jesteś w bashu, w kontenerze, w głównym folderze (root - `/`).

## Usunięcie starego łańcucha

Musimy usunąć plik starego łańcucha - będziemy synchronizować się z blockchainem na nowo.

* Będąc w głównym folderze kontenera (`/`) wpisz polecenie:  
`rm -rf opt/neo-python/Chains/privnet`

## Opłaty sieci - informacja

Deploy kontraktów do sieci wymaga wniesienia opłaty - wdrażasz kontrakt za pomocą adresu portfela, więc portfel musi zawierać odpowiednią ilość środków:
* **100 GAS** - za utworzenie kontraktu
* **+400 GAS** - za funkcjonalność dostępu do trwałego magazynu danych (storage)
* **+500 GAS** - za funkcjonalność dynamicznego wywoływania (dynamic call)  

Dodatkowo sieć pobiera opłaty za używnie funkcjonalności systemu w trakcie wykonywania kontraktu. Przy tym trzeba pamiętać, że jeśli suma opłat danej operacji będziemniejsza od **10 GAS**, to operacja ta wykoanana będzie za darmo.

>Pełna lista opłat: <http://docs.neo.org/en-us/sc/systemfees.html>

Prywatna sieć pobiera takie same opłaty, więc musimy posiadac portfel, który ma odpowiednio dużo GASu.

[Następny krok - utworzenie portfela z milionem monet](w2_wallet.md)
 

