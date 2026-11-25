# A7 · Còpies de seguretat automàtiques

## Nom de la tasca (Què?)
Programar còpies de seguretat diàries de les carpetes compartides al disc extern i comprovar que es poden restaurar.

## Mòdul i RA (Per a què?)
- Mòdul: MP05 – Serveis en xarxa
- RA associat: MP05-RA1: Instal·la i configura serveis en xarxa i aplica mesures de seguretat.

## Modalitat (Com?)
Individual — Rol C (serveis i seguretat), amb revisió del Rol A.

## Producte entregable (Suport)
- Script de còpia `configuracio/copies/copia.sh` i línia de `crontab` a `configuracio/copies/crontab.txt`.
- Captures a `evidencies/`: `A7-copia.png` (còpia feta i registre) i `A7-restauracio.png` (fitxer esborrat i recuperat).

## Instruccions pas a pas
1. Escriure l'script `/usr/local/bin/copia.sh`, que fa `rsync -a` de `/srv/associacio` a `/mnt/copies/AAAA-MM-DD` i guarda un registre a `/var/log/copia.log`.
2. Afegir a l'script l'esborrat de les còpies de més de 14 dies.
3. Donar permisos d'execució i provar l'script a mà.
4. Programar-lo amb `crontab -e` cada dia a les 02:00.
5. Fer una prova de restauració: esborrar un fitxer de prova de la carpeta compartida i recuperar-lo des de la còpia.
6. Copiar l'script i el crontab al repositori i publicar les captures.

## Recursos necessaris
- Entorn simulat: màquina virtual `srv-rpi` amb les carpetes de l'associació a `/srv/associacio` i el disc de còpies muntat a `/mnt/copies` (A6).
- Eines `rsync` i `cron`.

## Durada i setmana (Quan?)
3 hores · Setmana 4 (01/02/2027 – 05/02/2027).

## Lloc de realització (On?)
Aula-taller d'informàtica (IES Simarro).

## Responsable (Qui?)
- Executa: Rol C – Serveis i seguretat.
- Revisa el resultat: Rol A – Maquinari.

## Instrument d'avaluació
Rúbrica MP05 (professorat). Criteris:
- [ ] `configuracio/copies/copia.sh` està publicat i fa la còpia amb data i registre (25 %).
- [ ] `crontab.txt` programa la còpia diària a les 02:00 (25 %).
- [ ] La captura mostra la carpeta de còpia creada a `/mnt/copies` i el registre sense errors (25 %).
- [ ] La captura de la restauració demostra que el fitxer esborrat s'ha recuperat (25 %).

## Issue GitHub associada
#8 · Còpies de seguretat automàtiques 

## Incidències registrades
Cap de moment.
