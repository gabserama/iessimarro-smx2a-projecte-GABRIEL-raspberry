# Cronograma — Servidor domèstic amb Raspberry Pi per a una associació

S1 11-15/01 · S2 18-22/01 · S3 25-29/01 · S4 01-05/02 · S5 08-12/02/2027

## Gantt previst

| Tasca (responsable) | Fitxa | Issue | Depén de | S1 | S2 | S3 | S4 | S5 |
|---------------------|-------|-------|----------|----|----|----|----|----|
| Estudi de requisits i pressupost (A) | A4 | #2 | — | ■ | | | | |
| Muntatge de la Raspberry Pi (A) | A1 | #3 | — | ■ | | | | |
| Instal·lació del sistema operatiu (B) | A2 | #4 | A1 | | ■ | | | |
| Preparació del disc extern (A) | A6 | #6 | A1 | | ■ | | | |
| Configuració de la xarxa: IP fixa i SSH (B) | A5 | #5 | A2 | | | ■ | | |
| Servei d'arxius compartits (C) | A3 | #7 | A5 | | | | ■ | |
| Seguretat bàsica: tallafocs, usuaris i SSH (C) | A8 | #9 | A5 | | | | ■ | |
| Còpies de seguretat automàtiques (C) | A7 | #8 | A6, A5 | | | | ■ | |
| Proves finals i documentació tècnica (B) | A9 | #10 | A3, A7, A8 | | | | | ■ |

Camí crític (cadena més llarga): A1 → A2 → A5 → A3 → A9, que ocupa les cinc setmanes sense marge.

## Gantt real

## Desviacions

