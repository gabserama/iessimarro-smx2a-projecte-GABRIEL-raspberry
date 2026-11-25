# A6 · Preparació del disc extern per a còpies

## Nom de la tasca (Què?)
Preparar el disc extern on es guardaran les còpies de seguretat: crear la partició, formatar-la i muntar-la automàticament en arrencar.

## Mòdul i RA (Per a què?)
- Mòdul: MP01 – Muntatge i manteniment d'equips
- RA associat: MP01-RA1: Munta equips microinformàtics i en verifica el funcionament.

## Modalitat (Com?)
Individual — Rol A (maquinari), amb revisió del Rol B.

## Producte entregable (Suport)
- Procediment i línia de muntatge a `configuracio/disc/A6-disc.md` (inclou la línia de `/etc/fstab`).
- Captures a `evidencies/`: `A6-lsblk.png` (disc i partició) i `A6-muntatge.png` (`df -h` després de reiniciar).

## Instruccions pas a pas
1. Afegir a la màquina virtual un segon disc virtual de 8 GB que fa de disc extern USB.
2. Identificar el disc amb `lsblk` i crear-hi una partició amb `fdisk`.
3. Formatar la partició en ext4 amb l'etiqueta `copies`: `sudo mkfs.ext4 -L copies /dev/sdb1`.
4. Crear el punt de muntatge `/mnt/copies` i obtenir l'UUID amb `blkid`.
5. Afegir la línia a `/etc/fstab` amb l'UUID i l'opció `nofail`, i comprovar-la amb `sudo mount -a`.
6. Reiniciar i verificar amb `df -h` que el disc es munta sol.

## Recursos necessaris
- Entorn simulat: segon disc virtual (VDI de 8 GB) connectat a la màquina virtual `srv-rpi`, que representa el disc USB d'1 TB. El VDI no es puja al repositori.
- Eines `lsblk`, `fdisk`, `mkfs.ext4` i `blkid`.

## Durada i setmana (Quan?)
3 hores · Setmana 2 (18/01/2027 – 22/01/2027).

## Lloc de realització (On?)
Aula-taller d'informàtica (IES Simarro).

## Responsable (Qui?)
- Executa: Rol A – Maquinari.
- Revisa el resultat: Rol B – Sistema i xarxa.

## Instrument d'avaluació
Rúbrica MP01 (professorat). Criteris:
- [ ] La captura de `lsblk` mostra el disc amb la partició creada (25 %).
- [ ] La partició està formatada en ext4 amb l'etiqueta `copies` (25 %).
- [ ] `configuracio/disc/A6-disc.md` conté la línia de `fstab` amb UUID i `nofail` (25 %).
- [ ] La captura de `df -h` després de reiniciar mostra `/mnt/copies` muntat (25 %).

## Issue GitHub associada
#6 · Preparació del disc extern per a còpies

## Incidències registrades
Cap de moment.
