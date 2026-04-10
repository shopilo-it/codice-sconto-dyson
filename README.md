# Codice sconto Dyson, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Dyson** da [shopilo.it](https://shopilo.it/negozi/dyson.it). Restituisce **coupon Dyson** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-dyson](https://shopilo-it.github.io/codice-sconto-dyson/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-dyson
cd codice-sconto-dyson
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Dyson",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su aspirapolvere e purificatori",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/dyson.it"
  }
]
```

## Coupon Dyson disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su aspirapolvere e purificatori | [shopilo.it](https://shopilo.it/negozi/dyson.it) |

Codici attivi: **[shopilo.it/negozi/dyson.it](https://shopilo.it/negozi/dyson.it)**

## Domande frequenti

### Come utilizzo un codice sconto Dyson?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/dyson.it), aggiungi i prodotti al carrello su Dyson e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Dyson?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Dyson piu recenti?
La pagina [shopilo.it/negozi/dyson.it](https://shopilo.it/negozi/dyson.it) viene aggiornata quotidianamente con i codici sconto Dyson, voucher Dyson e coupon promozionali Dyson piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Dyson

Dyson e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/dyson.it) trovi i migliori codici sconto Dyson, coupon Dyson verificati e voucher Dyson attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-dyson
```

```javascript
const { fetchCoupons } = require('codice-sconto-dyson');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
