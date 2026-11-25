# A5 · Configuració de la xarxa (IP fixa i SSH)

## Nom de la tasca (Què?)
Assignar una adreça IP fixa al servidor i habilitar l'accés remot per SSH perquè es puga administrar sense pantalla ni teclat.

## Mòdul i RA (Per a què?)
- Mòdul: MP03 – Sistemes operatius
- RA associat: MP03-RA1: Instal·la i configura sistemes operatius i les seues xarxes bàsiques.

## Modalitat (Com?)
Individual — Rol B (sistema i xarxa), amb revisió del Rol C.

## Producte entregable (Suport)
- Fitxer de configuració de xarxa `configuracio/xarxa/interfaces`.
- Pla d'adreçament a `configuracio/xarxa/adrecament.md`.
- Captures a `evidencies/`: `A5-ip-fixa.png` (`ip a`) i `A5-ssh-client.png` (connexió SSH des del client).

## Instruccions pas a pas
1. Definir el pla d'adreçament: servidor 192.168.50.10/24, client 192.168.50.20/24 i porta d'enllaç 192.168.50.1.
2. Configurar la IP fixa a `/etc/network/interfaces` i reiniciar la xarxa.
3. Comprovar l'adreça amb `ip a` i la connectivitat amb `ping` des del client.
4. Instal·lar i activar el servidor SSH: `sudo apt install openssh-server -y`.
5. Connectar des del client amb `ssh usuari@192.168.50.10`.
6. Copiar la configuració al repositori i publicar les captures.

## Recursos necessaris
- Entorn simulat: màquina virtual `srv-rpi` i un client connectats a una xarxa interna de VirtualBox (`xarxa-associacio`).
- Paquet `openssh-server`.

## Durada i setmana (Quan?)
3 hores · Setmana 3 (25/01/2027 – 29/01/2027).

## Lloc de realització (On?)
Aula d'informàtica (IES Simarro).

## Responsable (Qui?)
- Executa: Rol B – Sistema i xarxa.
- Revisa el resultat: Rol C – Serveis i seguretat.

## Instrument d'avaluació
Rúbrica MP03 (professorat). Criteris:
- [ ] El pla d'adreçament està publicat i és coherent amb la configuració (25 %).
- [ ] `configuracio/xarxa/interfaces` defineix la IP fixa 192.168.50.10 (25 %).
- [ ] La captura de `ip a` i el `ping` des del client demostren la connectivitat (25 %).
- [ ] La captura mostra una sessió SSH oberta des del client (25 %).

## Issue GitHub associada
#5 · Configuració de la xarxa (IP fixa i SSH) 

## Incidències registrades
Cap de moment.
