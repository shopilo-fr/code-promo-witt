# Code promo Witt, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Witt** depuis [shopilo.fr](https://shopilo.fr/reductions/witt.fr). Renvoie les **coupons Witt** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-witt](https://shopilo-fr.github.io/code-promo-witt/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-witt
cd code-promo-witt
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Witt",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur la mode femme grandes tailles",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/witt.fr"
  }
]
```

## Coupons Witt disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur la mode femme grandes tailles | [shopilo.fr](https://shopilo.fr/reductions/witt.fr) |

Codes actifs : **[shopilo.fr/reductions/witt.fr](https://shopilo.fr/reductions/witt.fr)**

## Questions frequentes

### Comment utiliser un code promo Witt ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/witt.fr), ajoutez les produits a votre panier sur Witt et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Witt ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Witt les plus recents ?
La page [shopilo.fr/reductions/witt.fr](https://shopilo.fr/reductions/witt.fr) est mise a jour quotidiennement avec les codes promo Witt, bons de reduction Witt et coupons promotionnels Witt les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Witt

Witt est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/witt.fr), retrouvez les meilleurs codes promo Witt, coupons Witt verifies et bons de reduction Witt actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-witt
```

```javascript
const { fetchCoupons } = require('code-promo-witt');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
