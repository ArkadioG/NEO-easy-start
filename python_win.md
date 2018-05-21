# Instalacja Python 3.6 na Windows

1. Pobierz i zapisz plik:
    * [wersja 64bit](https://www.python.org/ftp/python/3.6.5/python-3.6.5-amd64.exe)
    * [wersja 32 bit](https://www.python.org/ftp/python/3.6.5/python-3.6.5.exe)
    
2. Uruchom instalator
3. na pierwszym ekranie kliknij opcję Customize installation
4. na drugim ekranie **Optional features** zaznacz wszystkie opcje **oprócz**  
    `Download debugging symbols`  oraz  
    `Download debug binaries`
5. na trzecim ekranie "Advanced Options" zaznacz nastęujące opcje:  
   `Associate files with Python`  
    `Create shortcuts for installed Applications`  
    `Add Python to environment variables` **WAŻNE**

6. sprawdź jakim poleceniem będziesz uruchamiać Python 3.6 (jeśli nie miałeś wcześniej innej wersji zainstalowanej to będzie to `python`)
    * wpisz polecenie `python -V`  
        * jeśli w odpowiedzi uzyskałeś `Python 3.6.5` to w dalszej części warsztatu używaj polecenia `python`
        * jeśli był inny rezultat to sprawdź polecenia `python3 -V` oraz `python3.6 -V` i zapamiętaj, która dałą rezultat `Python 3.6.5`
    
