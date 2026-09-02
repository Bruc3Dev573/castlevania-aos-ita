# Castlevania: Aria of Sorrow - Italian Enhanced Edition

[English](README.md) · **Italiano**

Italian Enhanced Edition non ufficiale di *Castlevania: Aria of Sorrow* per Game Boy Advance, con traduzione italiana, colori rivisti e modifiche di gioco opzionali.

## Contenuto di tutte le varianti

- **[Traduzione italiana v2.0](https://romhacking.it/project/view/id/190)** di Evrain.
- **[Colour Improvement v1.2](https://www.romhacking.net/hacks/9121/)** di Piggy Chan!, portata dalla ROM USA alla ROM europea.
- **[Correzione INT](https://www.romhacking.net/hacks/5645/)** di Dev Anj: le anime Bullet beneficiano correttamente della statistica INT di Soma.
- **[Correzione LCK](https://www.romhacking.net/hacks/5645/)** di Dev Anj: LCK influisce in modo significativo sulla probabilità di ottenere oggetti e anime.

Le varianti opzionali aggiungono:

- **[MP Regen](https://www.romhacking.net/hacks/5645/)** di Dev Anj: aumenta la velocità di rigenerazione degli MP.
- **[Better Drops](https://github.com/Xanthus1/aos_patches)** di Xanthus: aumenta le probabilità base di ottenere oggetti e anime.

Ogni patch è cumulativa: applica un solo file direttamente alla ROM europea pulita. Tutte le varianti includono già i quattro componenti elencati sopra.

## Varianti

| Variante | Modifiche aggiuntive | Impatto sul bilanciamento | Patch |
|---|---|---|---|
| Standard | Nessuna | La più vicina al bilanciamento originale | [`castlevania-aos-ita-v1.0.0.ips`](patches/castlevania-aos-ita-v1.0.0.ips) |
| MP Regen | Rigenerazione MP accelerata | Scontri lunghi più facili, con anime utilizzabili più spesso | [`castlevania-aos-ita-v1.0.0-mp.ips`](patches/castlevania-aos-ita-v1.0.0-mp.ips) |
| Better Drops | Probabilità base più alte per oggetti e anime | Meno farming | [`castlevania-aos-ita-v1.0.0-drop.ips`](patches/castlevania-aos-ita-v1.0.0-drop.ips) |
| Completa | MP Regen e Better Drops | La più permissiva, con entrambi i vantaggi | [`castlevania-aos-ita-v1.0.0-mp-drop.ips`](patches/castlevania-aos-ita-v1.0.0-mp-drop.ips) |

MP Regen proviene dall'archivio originale di Dev Anj. Better Drops usa le sei modifiche opzionali alle soglie dei drop della patch [LCK Plus Better Drop Rates](https://github.com/Xanthus1/aos_patches) di Xanthus. Queste modifiche non fanno parte della correzione LCK standard.

### Hash delle ROM risultanti

- Standard: `9300CC40EC53AB8C0C30067928E017163F836887198363B3DC7AAB0C12DEB630`
- MP Regen: `5DF1D21C383DF914274744F82CE8F1BDE880624CF308651705E6E8522E8C022B`
- Better Drops: `9308FAA239C38EF1FDCEBB7E41011443AB648AFC6C53C976FE36DF4AE5BF48B7`
- Completa: `3A4DE409EC8427AF86CAF10FE856F1A1B204D690899DEE69B300C959E2260A16`

## ROM richiesta

Applica la patch direttamente a una ROM europea pulita che corrisponda a tutti questi valori:

| Proprietà | Valore atteso |
|---|---|
| Titolo | `Castlevania - Aria of Sorrow (Europe) (En,Fr,De)` |
| Codice gioco | `A2CP` |
| CRC32 | `D0C91F74` |
| SHA-1 | `2E8302C2A5A61614749F609D7EDC8C3E6AF20585` |

Non applicare la patch alla ROM USA o a una ROM già modificata.

## Installazione

1. Verifica che la ROM corrisponda agli hash indicati sopra.
2. Crea una copia di sicurezza del file originale.
3. Scegli una variante dalla tabella e applica quella patch IPS con [Lunar IPS](https://fusoya.eludevisibility.org/lips/) o un altro programma compatibile.
4. Avvia la ROM ottenuta nel tuo emulatore preferito o su hardware compatibile.

Confronta la ROM risultante con lo SHA-256 indicato per la variante scelta.

## Verifica

Ogni patch produce la ROM indicata nella tabella delle varianti.

INT e LCK sono state verificate con test mirati in emulatore. La variante Standard ha inoltre completato entrambe le fasi dello scontro con Chaos ed è arrivata al frame 20.001 senza crash. Le varianti MP e Completa hanno superato uno smoke test di avvio.

I test hanno coperto i sistemi modificati e una sequenza di fine gioco, non l'intera partita.

## Crediti

- **Evrain:** traduzione italiana v2.0.
- **OldHouse, IKKI_THE_FENIX e Il Pulciaro:** beta testing della traduzione originale.
- **_Scorpio_:** assistenza nel ROM hacking della traduzione originale.
- **Brisma:** informazioni sui puntatori GBA per la traduzione originale.
- **Clomax e Tidus:** ringraziamenti speciali nel readme originale della traduzione.
- **Piggy Chan!:** Colour Improvement v1.2.
- **Dev Anj:** patch originali INT, LCK e MP Regen.
- **Rabite:** documentazione e pubblicazione autorizzata delle patch di Dev Anj.
- **Xanthus:** modifiche opzionali Better Drops.
- **Bruc3Dev573:** integrazione europea, preparazione delle patch e verifica.

Il permesso di ridistribuzione e la descrizione originale delle correzioni di Dev Anj sono conservati integralmente in [`docs/DevAnj-LCKFix-license-readme.txt`](docs/DevAnj-LCKFix-license-readme.txt).

Le condizioni di attribuzione e ridistribuzione del materiale originale del progetto sono descritte in [`NOTICE`](NOTICE).

## Note legali

Questo è un progetto amatoriale non ufficiale e non commerciale. Konami e gli autori originali non sono coinvolti. Il repository contiene soltanto patch, checksum e documentazione. Non contiene ROM o salvataggi.

È necessario possedere una copia legittima del gioco. I titolari dei diritti e gli autori originali possono richiedere correzioni, modifiche ai crediti o la rimozione tramite GitHub Issues.
