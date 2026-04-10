# Cod reducere Dyson — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Dyson** de pe [shopilo.it](https://shopilo.it/magazin/dyson.it). Returneaza **cupoane Dyson** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-dyson](https://shopilo-it.github.io/codice-sconto-dyson/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-dyson
cd codice-sconto-dyson
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Dyson",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su aspirapolvere e purificatori",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/dyson.it"
  }
]
```

## Cupoane Dyson disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% di sconto su aspirapolvere e purificatori | [shopilo.it](https://shopilo.it/magazin/dyson.it) |

Codurile active: **[shopilo.it/magazin/dyson.it](https://shopilo.it/magazin/dyson.it)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Dyson?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/dyson.it), adauga produsele in cos pe Dyson, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Dyson?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Dyson?
Pagina [shopilo.it/magazin/dyson.it](https://shopilo.it/magazin/dyson.it) este actualizata zilnic cu cele mai noi cod reducere Dyson, voucher Dyson si cupon promotional Dyson.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Dyson

Dyson este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/dyson.it) cele mai bune cod reducere Dyson, cupoane Dyson verificate si voucher Dyson active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-dyson
```

```javascript
const { fetchCoupons } = require('codice-sconto-dyson');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
