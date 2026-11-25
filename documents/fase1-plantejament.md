# Fase 1 · Plantejament inicial — Servidor domèstic amb Raspberry Pi per a una associació

## Necessitat detectada

Una associació xicoteta del barri comparteix els documents per correu electrònic i en memòries USB.
No té còpies de seguretat ni control d'accés, i això provoca pèrdues d'informació i posa en risc 
les dades dels socis. L'associació té poc pressupost i no pot contractar un servidor professional.

## Idees inicials

| # | Idea | Necessitat que resol (qui i per què) | Mòduls implicats |
|---|------|--------------------------------------|------------------|
| 1 | Servidor domèstic amb Raspberry Pi | L'associació necessita compartir arxius i fer còpies de 
seguretat amb poc pressupost | MP01, MP03, MP05 |
| 2 | (IDEA 2 DE LA PRÀCTICA 3) | (qui la necessita i per què) | (mòduls) |
| 3 | (IDEA 3 DE LA PRÀCTICA 3) | (qui la necessita i per què) | (mòduls) |

## Idea triada i justificació

S'ha triat la idea 1 perquè resol un problema real i proper (pèrdua de documents i falta de còpies),
té un cost molt reduït i es pot fer en les cinc setmanes previstes. Compleix els criteris de 
qualitat: és rellevant, permet repartir el treball en tres rols, té marge per a la creativitat i és
un treball habitual en una empresa de serveis informàtics.

## Organització destinatària

- Tipus d'organització: associació sense ànim de lucre (associació de barri).
- Activitat principal: activitats socials i culturals per als socis del barri.
- Persones i organització interna: una junta directiva (presidència, secretaria i tresoreria) i un 
grup de voluntaris que gestionen els documents de l'associació.
- Situació informàtica actual: portàtils personals dels voluntaris, el router de l'operador d'Internet
i documents repartits entre correus i memòries USB, sense servidor, sense còpies de seguretat i sense control d'accés.

## Empresa que executaria el projecte

- Tipus d'empresa del sector: xicoteta empresa de serveis informàtics i manteniment per a particulars,
associacions i pimes.
- Serveis que ofereix: muntatge i reparació d'equips, instal·lació de sistemes operatius, configuració
de xarxes locals, servidors d'arxius, còpies de seguretat i manteniment.
- Perfils professionals de SMX implicats: tècnic/a de muntatge i manteniment d'equips, tècnic/a de
sistemes i xarxes i tècnic/a de suport i seguretat informàtica.

## Mòduls i RA preliminars

- MP01 (Muntatge i manteniment d'equips): RA1 · Munta equips microinformàtics i en verifica el
funcionament.
- MP03 (Sistemes operatius): RA1 · Instal·la i configura sistemes operatius i les seues xarxes
bàsiques.
- MP05 (Serveis en xarxa): RA1 · Instal·la i configura serveis en xarxa i aplica mesures de seguretat.
- Projecte Intermodular: RA1 i RA2.

## Viabilitat inicial

- Temps: 5 setmanes d'execució (de l'11/01/2027 al 12/02/2027).
- Pressupost aproximat: entre 150 i 250 € de material, més la mà d'obra
(detall a documents/pressupost.md).
- Equipament: Raspberry Pi, targeta microSD, font d'alimentació, carcassa amb refrigeració, disc
extern USB i cable de xarxa.
- Programari lliure: Raspberry Pi OS, Samba, SSH, tallafocs UFW i rsync/cron per a les còpies.




