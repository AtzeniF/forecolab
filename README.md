# Sito del ForEcoLab

Sito del Forest Ecology and Tree-Ring Laboratory (D3A, Università Politecnica delle Marche), pubblicato con GitHub Pages.

## Come si aggiorna

I testi non stanno nel codice ma in `_data/`:

| File | Cosa contiene |
|---|---|
| `_data/team.yml` | persone, gruppo, tema, ORCID |
| `_data/temi.yml` | temi di ricerca con la loro foto |
| `_data/metodi.yml` | i capitoli con le foto grandi |
| `_data/strumenti.yml` | strumenti del laboratorio |
| `_data/sito.yml` | titoli, frasi, email e foto delle sezioni |
| `_progetti/*.md` | un file per progetto: la riga in home e la sua pagina `/progetti/<nome-file>/` |

Il modo più semplice è **Pages CMS**: si entra su https://app.pagescms.org con l'account GitHub, si apre questo repository e si modificano i moduli. Ogni salvataggio aggiorna il sito in circa un minuto. Le foto caricate finiscono in `assets/img/`: meglio caricarle già ridotte (lato lungo 1600-2000 px, sotto i 400 KB).

## Struttura

- `index.html`: la home, un template Jekyll che legge `_data/` e `_progetti/`.
- `_layouts/progetto.html`: la pagina di ogni progetto.
- `assets/`: stili, script e immagini (dal kit di design usato per costruire la pagina).
- `.pages.yml`: i moduli di Pages CMS.
- `credits.html`: crediti delle foto Wikimedia Commons usate come segnaposto.
