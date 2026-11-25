# Document de Repte - Servidor domestic amb raspberry pi per a una associacio

## Titol del projecte
Servidor domestic amb raspberry pi per a una associacio

## Grup i membres 
-AlumneA: Rol A - maquinari: muntatge i preparacio de la raspberry pi

-AlumneB: Rol B - sistema i xarxa: instalacio del sistema operatiu i configuracio de la xarxa

-AlumneC: Rol C - serveis i seguretat: arxius compartits,copies de seguretat i proteccio

-Projecte realitzat individualment per GABRIEL (rols simulats)

## Centre i curs

IES Simarro - SMX 2n A - Curs 2026-2027


## Context i situacio inicial

Una associacio xicoteta del barri comparteix documents per correu i en memories USB,sense copies de seguretat ni control
de acces. Aixo provoca perdua de informacio i risc per a les dades dels socis. La associacio disposa de poc pressupost
i no pot contractar un servidor professional.

## Repte proposat

Dissenyar i implementar un servidor domestic basat en una raspberry pi que permeta a la associacio compartir arxius,
fer copies de seguretat automatiques i protegir les seues dades,amb un cost reduit.

## Objectiu general

Implementar un servidor domèstic de baix cost basat en una Raspberry Pi que permeta a l'associació 
compartir arxius de manera segura i disposar de còpies de seguretat automàtiques.

## Objectius especifics
1.Muntar i preparar el maquinari de la raspberry pi i el disc extern.
2.Instalar el sistema operatiu i configurar la xarxa amb IP fixa i acces SSH.
3.Configurar un servei de arxius compartits amb permisos per usuari.
4.Programar copies de seguretat automatiques i comprovarne la restauracio.
5.Aplicar mesures de seguretat basiques: tallafocs, usuaris i SSH amb clau.

## Moduls professionals implicats
-MP01 (Maquinari)
-MP03 (Sistemes)
-MP05 (Serveis)

## RA associats per modul
- MP01-RA1: Munta equips microinformatics i en verifica el funcionament.
- MP03-RA1: Instala i configura sistemes operatius i les seues xarxes basiques.
- MP05-RA1: Instala i configura serveis en xarxa i aplica mesures de seguretat.


## Criteris d'avaluació per RA

| Mòdul | RA | Criteri d'avaluació | Tasca que l'evidencia |
|-------|----|---------------------|-----------------------|
| MP01 | RA1 | La Raspberry Pi està muntada amb refrigeració i arranca correctament | #3 · Muntatge 
de la Raspberry Pi |
| MP01 | RA1 | El disc extern està formatat i es munta automàticament | #6 · Preparació del disc
extern per a còpies |
| MP03 | RA1 | El sistema operatiu està instal·lat i actualitzat | #4 · Instal·lació del sistema
operatiu |
| MP03 | RA1 | El servidor té IP fixa i s'hi accedeix per SSH | #5 · Configuració de la xarxa
(IP fixa i SSH) |
| MP05 | RA1 | La carpeta compartida funciona amb permisos per usuari | #7 · Servei d'arxius
compartits |
| MP05 | RA1 | Les còpies automàtiques s'executen i es poden restaurar | #8 · Còpies de seguretat
automàtiques |
| MP05 | RA1 | El tallafocs, els usuaris i l'SSH amb clau estan configurats | #9 · Seguretat
bàsica: tallafocs, usuaris i SSH |
| PI | RA2 | El pressupost és realista i compara proveïdors | #2 · Estudi de requisits i pressupost
del maquinari |

## Criteris de qualitat del repte
- Proximitat/rellevancia: Si
- Treball en equip: Si
- Creativitat: Si
- Connexio profesional: Si

## Requeriments tecnics
- Hardware: Raspberry Pi, targeta microSD, font de alimentacio,carcasa amb refrigeracio,disc extern USB,cable de xarxa.
- Programari: Raspberry PI OS, servei de arxius compartits (Samba), SSH, tallafocs,eina de copies programades.

## Limitacions o restriccions
- Pressupost reduit de la associacio
- Espai limitat al local de la associacio
- Temps: 5 setmanes (del 11.01.27 al 12.02.27)
- Equipament limitat a una raspberry pi i un disc extern.
