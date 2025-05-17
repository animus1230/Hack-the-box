# Notatka z nauki – HackTheBox (Pentest podstawy)

## Komendy i ich zastosowanie (prosto i na temat):

### Skanowanie i połączenia:
ping IP                       – sprawdzenie, czy host odpowiada
nmap -p- IP                   – skanowanie wszystkich portów
telnet IP 23                  – połączenie z otwartym portem Telnet (23)

### Identyfikacja użytkownika:
whoami                        – pokazuje nazwę użytkownika
id                            – pokazuje UID, GID i grupy (UID=0 to root)
ls -la                        – pokazuje pliki, w tym ukryte
cat plik                      – podgląd zawartości pliku

### Uprawnienia i historia:
sudo -l                       – sprawdzenie, jakie komendy możemy wykonać z sudo
cat ~/.bash_history           – pokazuje historię komend użytkownika (czasem są tam hasła!)

### Zaplanowane zadania:
cat /etc/crontab              – pokazuje automatyczne zadania uruchamiane przez system

### Informacje o systemie:
netstat -tuln                 – pokazuje, jakie usługi nasłuchują (porty)
ss -tulnp                     – nowoczesna wersja netstat, pokazuje też PID programu

### Wyszukiwanie:
find / -name "*.log"          – szukanie plików logów (mogą zawierać cenne dane)
find / -perm -4000            – wyszukiwanie plików z SUID (mogą pozwolić na przejęcie roota)

## Co osiągnięto:
- Zalogowano się przez Telnet jako root
- Sprawdzono użytkownika i jego uprawnienia
- Znaleziono pliki, flagi, potencjalne dane dostępowe
- Zrozumiano podstawy hakowania systemu lokalnie.
- właśnie tego sie nauczyłem dzisiaj i każdego dznia staje sie coraz lepszy 
