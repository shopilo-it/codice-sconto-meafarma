# Codice sconto Meafarma, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Meafarma** da [shopilo.it](https://shopilo.it/negozi/meafarma.it). Restituisce **coupon Meafarma** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-meafarma](https://shopilo-it.github.io/codice-sconto-meafarma/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-meafarma
cd codice-sconto-meafarma
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Meafarma",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su prodotti farmaceutici online",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/meafarma.it"
  }
]
```

## Coupon Meafarma disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su prodotti farmaceutici online | [shopilo.it](https://shopilo.it/negozi/meafarma.it) |

Codici attivi: **[shopilo.it/negozi/meafarma.it](https://shopilo.it/negozi/meafarma.it)**

## Domande frequenti

### Come utilizzo un codice sconto Meafarma?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/meafarma.it), aggiungi i prodotti al carrello su Meafarma e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Meafarma?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Meafarma piu recenti?
La pagina [shopilo.it/negozi/meafarma.it](https://shopilo.it/negozi/meafarma.it) viene aggiornata quotidianamente con i codici sconto Meafarma, voucher Meafarma e coupon promozionali Meafarma piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Meafarma

Meafarma e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/meafarma.it) trovi i migliori codici sconto Meafarma, coupon Meafarma verificati e voucher Meafarma attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-meafarma
```

```javascript
const { fetchCoupons } = require('codice-sconto-meafarma');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
