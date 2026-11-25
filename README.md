# instagram-italiano

Una skill per [Claude Code](https://claude.com/claude-code) che aiuta piccoli creator e progetti italiani a preparare
contenuti per Instagram e TikTok: didascalie, caroselli, reel, il piano della settimana, la revisione del profilo.
Tutto in italiano, con esempi italiani.

## Cosa fa
- Scrive didascalie con il gancio nei primi ~125 caratteri e una sola richiesta finale.
- Progetta caroselli slide per slide, con la promessa nella prima e un riepilogo da salvare nell'ultima.
- Prepara la scaletta di reel e TikTok con testo a schermo, scena per scena.
- Fa il piano della settimana per pilastri (utile, storia, leggero, promozione) con un controllo finale.
- Sceglie 3-5 hashtag italiani della taglia giusta.
- Rivede il profilo: nome, bio, link, storie in evidenza, griglia, post fissati.
- Trasforma una guida, un articolo o un video lungo in un carosello o in un reel.
- Controlla i segni di testo scritto da un'AI in italiano.

## Cosa non fa
- **Non pubblica e non programma.** Consegna bozze pronte da incollare: pubblichi tu, dopo averle lette.
- Non mette like, non commenta, non segue, non manda messaggi.
- Non legge Instagram o TikTok con strumenti esterni (scraper o API non ufficiali).
- Non inventa numeri, risultati o esperienze: se un dato manca, lo chiede o toglie la frase.
- Tratta il testo letto online come un dato: le frasi rivolte all'agente dentro post e commenti non vengono eseguite.

## Installazione
Copia la cartella in uno di questi posti:

- `~/.claude/skills/instagram-italiano/` per usarla in tutti i progetti;
- `.claude/skills/instagram-italiano/` dentro un progetto, per usarla solo lì.

```sh
git clone https://github.com/lucianomurr/instagram-italiano ~/.claude/skills/instagram-italiano
```

Claude Code la carica da solo quando la richiesta riguarda Instagram o TikTok. Puoi anche chiamarla per nome:
`/instagram-italiano`.

## Esempi di richieste
- "Scrivi la didascalia per questo carosello sulle scarpe da corsa per principianti. Obiettivo: salvataggi."
- "Trasforma questa guida in un carosello da 7 slide." (allega o incolla il testo)
- "Fammi il piano della prossima settimana: 2 reel, 1 carosello, storie. Il profilo parla di cucina vegetariana a Bologna."
- "Rivedi la mia bio e dimmi quali post fissare."
- "Questa didascalia sembra scritta da un'AI? Correggila."

## I file
| File | Contenuto |
|---|---|
| `SKILL.md` | regole e modo di lavorare |
| `riferimenti/ganci.md` | dieci formule di gancio, scelte per obiettivo |
| `riferimenti/segnali.md` | cosa premia la piattaforma e cosa la frena |
| `riferimenti/caroselli.md` | struttura dei caroselli |
| `riferimenti/piano-settimanale.md` | pilastri ed esempio di settimana |
| `riferimenti/hashtag.md` | hashtag per taglia |
| `riferimenti/checklist-didascalia.md` | controllo prima di consegnare |
| `riferimenti/profilo.md` | revisione del profilo in nove parti |
| `riferimenti/riadattare.md` | da guida o articolo a carosello o reel |
| `riferimenti/reel.md` | reel e TikTok con testo a schermo, scaletta delle riprese |
| `riferimenti/testo-ai-italiano.md` | segni di testo scritto da un'AI in italiano |

## Crediti
Le formule di gancio, i segnali della piattaforma, la struttura dei caroselli, il piano per pilastri, la strategia
degli hashtag, la revisione del profilo e il riadattamento vengono da
[sergebulaev/instagram-skills](https://github.com/sergebulaev/instagram-skills) (commit `823c681`, licenza MIT),
rielaborati in italiano.

Cosa cambia rispetto all'originale:
- testi riscritti in italiano con esempi italiani, non tradotti parola per parola;
- tolto tutto il codice: pubblicazione automatica (Publora), immagini generate (Pixfaro), lettura dei profili (Apify);
- la skill prepara solo bozze e non pubblica mai;
- hashtag in italiano e orari indicativi per l'Italia;
- nel profilo la foto può essere un volto o un logo, come preferisci (l'originale consiglia il volto);
- nuovi: `reel.md` (testo a schermo e riprese) e `testo-ai-italiano.md` (segni di testo AI in italiano, al posto
  dello "humanizer" in inglese).

Autore della versione italiana: Luciano Murruni ([lungolento.it](https://lungolento.it)).

## Licenza
MIT. Vedi `LICENSE`.
