# Mała sieć z serwerem Windows i klientami.

## Opis projektu:
Projekt przedstawia konfigurację małej sieci firmowej z wykorzystaniem Windows Server 2022 oraz klientów Windows 11. Zawiera instalację Active Directory (AD), konfigurację serwera DHCP i DNS, a także dodanie komputerów do domeny.

Celem projektu jest nauka podstaw administracji Windows Server oraz zarządzania użytkownikami w środowisku domenowym.

## Technologie:
- Windows Server 2022 (serwer domeny)
- Windows 11 (klienci)
- VirtualBox (do uruchamiania maszyn wirtualnych)

## Kroki konfiguracji:
I. Instalacja Windows Server na maszynie wirtualnej
   1. Pobierz i zainstaluj Windows Server 2022
   2. Skonfiguruj statyczny adres IP dla serwera
   3. Pobierz i zainstaluj aktualizacje Serwera
   4. Zainstaluj rolę Active Directory Domain Services (AD DS)

II. Konfiguracja Active Directory
    1. Utwórz nową domenę: rafal.local
    2. Skonfiguruj jednostki organizacyjne dla użytkowników i komputerów
    3. Dodaj użytkowników do domeny i przypisz im role

III. Konfiguracja DHCP i DNS:
     1. DNS - ustaw serwer DNS na rafal.local
     2. DHCP - skonfiguruj zakres adresów IP dla klientów
     3. Przetestuj, czy klienci pobierają adresy z DHCP

IV. Dodanie klientów do domeny:
    1. Skonfiguruj klienta (Windows) i ustaw jako członka domeny
    2. Zaloguj się na konto użytkownika domenowego
    3. Sprawdź dostęp do zasobów sieciowych

## Zrzuty ekranu:
   1. Konfiguracja AD DS na Windows Server
   2. Konfiguracja DHCP
   3. Dodanie klienta Windows do domeny

## Umiejętności zdobyte w projekcie:
   - Instalacja i konfiguracja Windows Server
   - Tworzenie i zarządzanie Active Directory
   - Konfiguracja DHCP i DNS
   - Dodawanie komputerów do domeny
   - Zarządzanie użytkownikami i uprawnieniami

## Struktura plików w repozytorium:
	mala-siec-z-serwerem-Windows-i-klientami/
	|-- README.md
	|-- screenshots/
	    |-- about-serwer.png
	    |-- install-WinServ.png
	    |-- AD-1.png
	    |-- AD-2.png
	    |-- dhcp.png
	    |-- DNS.png
	    |-- domena-1.png
	    |-- domena-2.png
	    |-- domena-3.png