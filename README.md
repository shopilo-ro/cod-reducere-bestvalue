# Cod reducere BestValue — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere BestValue** de pe [shopilo.ro](https://shopilo.ro/magazin/bestvalue.eu). Returneaza **cupoane BestValue** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-bestvalue](https://shopilo-ro.github.io/cod-reducere-bestvalue/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-bestvalue
cd cod-reducere-bestvalue
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "BestValue",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la electronice si electrocasnice",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/bestvalue.eu"
  }
]
```

## Cupoane BestValue disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la electronice si electrocasnice | [shopilo.ro](https://shopilo.ro/magazin/bestvalue.eu) |

Codurile active: **[shopilo.ro/magazin/bestvalue.eu](https://shopilo.ro/magazin/bestvalue.eu)**

## Intrebari frecvente

### Cum folosesc un cod de reducere BestValue?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/bestvalue.eu), adauga produsele in cos pe BestValue, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele BestValue?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri BestValue?
Pagina [shopilo.ro/magazin/bestvalue.eu](https://shopilo.ro/magazin/bestvalue.eu) este actualizata zilnic cu cele mai noi cod reducere BestValue, voucher BestValue si cupon promotional BestValue.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre BestValue

BestValue este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/bestvalue.eu) cele mai bune cod reducere BestValue, cupoane BestValue verificate si voucher BestValue active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-bestvalue
```

```javascript
const { fetchCoupons } = require('cod-reducere-bestvalue');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
