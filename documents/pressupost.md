# Pressupost — Servidor domèstic amb Raspberry Pi per a una associació

Data dels preus: 25/11/2026

Preus unitaris sense IVA (preu de botiga ÷ 1,21).

| Capítol | Partida | Quantitat | Preu unitari (€) | Import (€) | Font |
|---------|---------|-----------|------------------|------------|------|
| Equipament | Raspberry Pi 5 (4 GB) | 1 | 90,39 | 90,39 | RS Online |
| Equipament | Font d'alimentació oficial USB-C 27 W | 1 | 12,36 | 12,36 | LDLC |
| Equipament | Carcassa oficial Raspberry Pi 5 amb ventilador | 1 | 10,70 | 10,70 | LDLC |
| Equipament | Targeta microSD SanDisk Extreme GO 64 GB A2 | 1 | 23,96 | 23,96 | MediaMarkt |
| Equipament | Disc extern WD Elements 1 TB 2,5" USB 3.0 | 1 | 89,26 | 89,26 | PcComponentes |
| Xarxa | Cable de xarxa Lanberg Cat6 U/UTP 2 m | 1 | 4,21 | 4,21 | PcComponentes |
| Programari | Raspberry Pi OS, Samba, UFW, rsync | 1 | 0,00 | 0,00 | Programari lliure |
| Mà d'obra | Rol A · Maquinari (A1, disc extern, requisits) | 12 h | 20,00 | 240,00 | Preu tècnic/a SMX |
| Mà d'obra | Rol B · Sistema i xarxa (A2, xarxa, proves) | 12 h | 20,00 | 240,00 | Preu tècnic/a SMX |
| Mà d'obra | Rol C · Serveis i seguretat (A3, còpies, seguretat) | 12 h | 20,00 | 240,00 | Preu tècnic/a SMX |

**Base imposable:** 950,88 €
**IVA (21 %):** 199,68 €
**Total:** 1.150,56 €

Resum: material 230,88 € + mà d'obra 720,00 € (36 h) = 950,88 € sense IVA.

## Comparativa de la partida principal

| Opció | Proveïdor | Preu (€, IVA inclòs) | Garantia | Termini | Triada |
|-------|-----------|----------|----------|---------|--------|
| A | Raspberry Pi 5 4 GB · RS Online | 109,37 | 3 anys (garantia legal) | Segons estoc | Sí |
| B | Raspberry Pi 5 8 GB · RS Online | 160,34 | 3 anys (garantia legal) | Segons estoc | No |

Justificació de la tria: el servidor només ha d'executar Samba, SSH, el tallafocs i les còpies amb rsync, que consumeixen poca memòria, de manera que 4 GB són suficients. L'opció B costa uns 51 € més i només compensaria si en el futur s'hi volgueren afegir serveis pesats (núvol privat, contenidors o multimèdia). A més, el preu de les Raspberry Pi varia molt segons la botiga: a PcComponentes el model de 4 GB arriba a uns 171 €, per això s'ha triat el distribuïdor oficial RS Online.

