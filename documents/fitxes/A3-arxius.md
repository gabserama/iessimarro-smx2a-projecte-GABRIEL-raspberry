# A3 · Servei d'arxius compartits

**Incidència associada:** #7 · Servei d'arxius compartits

## Nom de la tasca (Què?)
Instal·lar i configurar Samba a la Raspberry Pi perquè les persones de l'associació puguen guardar i consultar documents en una carpeta compartida amb permisos diferenciats.

## Mòdul i RA (Per a què?)
- Mòdul: MP05 – Serveis
- RA associat: MP05-RA1: Instal·la i configura serveis en xarxa i aplica mesures de seguretat.

## Modalitat (Com?)
Treball individual. La tasca la lidera el Rol C (serveis i seguretat), amb revisió del Rol B.

## Producte entregable (Suport)
- Fitxer de configuració del servei i instruccions d'accés documentades a `configuracio/samba/`.
- Captures de la carpeta compartida i de les proves d'accés amb un usuari autoritzat.

## Instruccions pas a pas
1. Actualitzar els repositoris del sistema i instal·lar el paquet Samba.
2. Crear la carpeta que es compartirà i establir-ne el propietari i els permisos necessaris.
3. Crear o seleccionar els usuaris autoritzats i configurar la compartició al fitxer de configuració de Samba.
4. Reiniciar el servei, validar la configuració i provar l'accés des d'un altre equip de la xarxa.
5. Comprovar que els usuaris autoritzats poden llegir i escriure i que els no autoritzats no hi tenen accés.
6. Documentar els passos i les incidències al repositori.

## Recursos necessaris
- Raspberry Pi amb Raspberry Pi OS actualitzat i connexió a la xarxa local.
- Paquet Samba i eines de terminal per a administrar el servei.
- Un segon ordinador per a provar l'accés a la carpeta compartida.

## Durada i setmana (Quan?)
6 hores · Setmana 4 del projecte (01/02/2027–05/02/2027).

## Lloc de realització (On?)
Aula-taller d'informàtica del centre.

## Responsable (Qui?)
- Executa: Rol C – Serveis i seguretat.
- Revisa el resultat: Rol B – Sistema i xarxa.

## Instrument d'avaluació
Rúbrica MP05:
- [ ] Servei Samba instal·lat i actiu (25%).
- [ ] Carpeta compartida creada amb permisos adequats (25%).
- [ ] Accés remot provat amb usuaris autoritzats (25%).
- [ ] Restriccions d'accés verificades i configuració documentada (25%).
