# DHCP, DNS, Static Routing – Cisco Packet Tracer Lab

## Opis projektu

Laboratorium przedstawia konfigurację podstawowych usług sieciowych w symulatorze Cisco Packet Tracer: **DHCP**, **DNS** oraz **trasowanie statyczne**. Projekt pozwala na praktyczne przećwiczenie konfiguracji serwerów, urządzeń końcowych i trasowania w środowisku symulowanym.

---

## Topologia sieci (zamierzony cel labu)

![topology](images/topology.PNG)

Sieć składa się z dwóch routerów, przełączników, serwera DHCP/DNS, serwera WWW oraz kilku stacji roboczych. Połączenia między urządzeniami zostały wykonane zgodnie z założeniami projektu.

---

## Konfiguracja DHCP

- **Serwer DHCP** został skonfigurowany z odpowiednimi pulami adresów IP dla poszczególnych segmentów sieci.
- Skonfigurowano `ip helper-address` na interfejsach routerów, aby umożliwić przekazywanie żądań DHCP do serwera.
  
![dhcp-ip](images/dhcp-ip-config.PNG)
![dhcp-pools](images/dhcp-server-pools.PNG)
![topology](images/ip-helper-address.PNG)

---

## Konfiguracja DNS

- **Serwer DNS** obsługuje rekordy domenowe dla lokalnej sieci.
- Rekordy DNS zostały przypisane do odpowiednich adresów IP serwera WWW.
- Pliki konfiguracyjne:
  
![dns-ip](images/dns-ip-config.PNG)
![dns-records](images/dns-server-records.PNG)

---

## Statyczne trasowanie

- Na routerach skonfigurowano trasy statyczne, aby zapewnić komunikację między wszystkimi segmentami sieci.
- Pliki konfiguracyjne:
  
![r1-switch](images/R1-switch-connection.PNG)
![r2-switch](images/R2-swtich-connection.PNG)
![static-ip](images/static-routing.PNG)

---

## Konfiguracja serwera WWW

- Sprawdzono poprawność przydzielania adresów IP przez DHCP na stacjach roboczych
- Przetestowano rozwiązywanie nazw przez DNS oraz dostępność serwera WWW

![web-ip](images/Web-ip-config.PNG)
![power-on](images/web-server-power-on.PNG)
![check-web-page-pc](images/check-web-page-pc.PNG)

---

## Podsumowanie

Laboratorium pozwala zrozumieć i przećwiczyć podstawowe zagadnienia związane z konfiguracją usług DHCP, DNS oraz trasowania statycznego w środowisku Cisco Packet Tracer. Pliki konfiguracyjne oraz zrzuty ekranu pomagają krok po kroku przeprowadzić cały proces.
