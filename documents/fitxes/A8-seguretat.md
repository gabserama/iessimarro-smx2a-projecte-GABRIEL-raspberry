# A8 · Seguretat bàsica: tallafocs, usuaris i SSH

## Nom de la tasca (Què?)
Protegir el servidor amb un tallafocs que només permeta SSH i Samba, comptes d'usuari segurs i accés SSH amb clau en lloc de contrasenya.

## Mòdul i RA (Per a què?)
- Mòdul: MP05 – Serveis en xarxa
- RA associat: MP05-RA1: Instal·la i configura serveis en xarxa i aplica mesures de seguretat.

## Modalitat (Com?)
Individual — Rol C (serveis i seguretat), amb revisió del Rol B.

## Producte entregable (Suport)
- Regles del tallafocs a `configuracio/seguretat/ufw-status.txt` (eixida de `sudo ufw status verbose`).
- Fragment modificat de `configuracio/seguretat/sshd_config` (sense claus ni contrasenyes).
- Captures a `evidencies/`: `A8-ufw.png`, `A8-ssh-clau.png` (accés amb clau) i `A8-ssh-denegat.png` (contrasenya rebutjada).

## Instruccions pas a pas
1. Instal·lar UFW i definir la política per defecte: denegar l'entrada i permetre l'eixida.
2. Permetre només SSH (22/tcp) i Samba (perfil `Samba`) des de la xarxa 192.168.50.0/24 i activar el tallafocs.
3. Revisar els comptes: cada persona té el seu usuari, contrasenyes fortes i cap compte innecessari amb `sudo`.
4. Generar una parella de claus al client (`ssh-keygen`) i copiar la pública al servidor (`ssh-copy-id`).
5. A `/etc/ssh/sshd_config`, posar `PermitRootLogin no` i `PasswordAuthentication no`, i reiniciar SSH.
6. Comprovar l'accés amb clau i que l'accés amb contrasenya es rebutja, i publicar la configuració i les captures.

## Recursos necessaris
- Entorn simulat: màquina virtual `srv-rpi` i el client a la xarxa interna de VirtualBox.
- Paquets `ufw` i `openssh-server`.

## Durada i setmana (Quan?)
3 hores · Setmana 4 (01/02/2027 – 05/02/2027).

## Lloc de realització (On?)
Aula-taller d'informàtica (IES Simarro).

## Responsable (Qui?)
- Executa: Rol C – Serveis i seguretat.
- Revisa el resultat: Rol B – Sistema i xarxa.

## Instrument d'avaluació
Rúbrica MP05 (professorat). Criteris:
- [ ] `ufw-status.txt` mostra la política per defecte de denegar i només SSH i Samba permesos (25 %).
- [ ] El fragment de `sshd_config` té `PermitRootLogin no` i `PasswordAuthentication no` (25 %).
- [ ] La captura mostra l'accés SSH amb clau des del client (25 %).
- [ ] La captura mostra que l'accés amb contrasenya es rebutja (25 %).

## Issue GitHub associada
#9 · Seguretat bàsica: tallafocs, usuaris i SSH 

## Incidències registrades
Cap de moment.
