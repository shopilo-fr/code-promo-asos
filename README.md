# Code promo ASOS, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo ASOS** depuis [shopilo.fr](https://shopilo.fr/reductions/asos.com). Renvoie les **coupons ASOS** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-asos](https://shopilo-fr.github.io/code-promo-asos/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-asos
cd code-promo-asos
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "ASOS",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% de reduction sur une selection de vetements",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/asos.com"
  }
]
```

## Coupons ASOS disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 20% | 20% de reduction sur une selection de vetements | [shopilo.fr](https://shopilo.fr/reductions/asos.com) |

Codes actifs : **[shopilo.fr/reductions/asos.com](https://shopilo.fr/reductions/asos.com)**

## Questions frequentes

### Comment utiliser un code promo ASOS ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/asos.com), ajoutez les produits a votre panier sur ASOS et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons ASOS ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction ASOS les plus recents ?
La page [shopilo.fr/reductions/asos.com](https://shopilo.fr/reductions/asos.com) est mise a jour quotidiennement avec les codes promo ASOS, bons de reduction ASOS et coupons promotionnels ASOS les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de ASOS

ASOS est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/asos.com), retrouvez les meilleurs codes promo ASOS, coupons ASOS verifies et bons de reduction ASOS actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-asos
```

```javascript
const { fetchCoupons } = require('code-promo-asos');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
