# legal

Documents légaux publics de Johann Hospice, servis par GitHub Pages sur https://johannhospice.github.io/legal/. Ce dépôt est la seule source : il remplace `techwithjohann-legal` et `fortuna-legal`.

## Pages

| Page | URL | Ancres |
| --- | --- | --- |
| Accueil | https://johannhospice.github.io/legal/ | |
| Johann \| Tech, outil de messages Instagram | https://johannhospice.github.io/legal/techwithjohann/ | `#suppression`, `#data-deletion` |
| Fortuna | https://johannhospice.github.io/legal/fortuna/ | `#confidentialite`, `#conditions`, `#privacy`, `#terms` |

## Qui pointe vers quoi

| Service | Champ | Adresse à déclarer | Adresse déclarée au 7/11/2026 | Qui change |
| --- | --- | --- | --- | --- |
| Meta, app « Tech with Johann » | Politique de confidentialité | `https://johannhospice.github.io/legal/techwithjohann/` | `https://johannhospice.github.io/techwithjohann-legal/` | Johann, ou la session Création avec son accord |
| Meta, app « Tech with Johann » | Instructions de suppression des données | `https://johannhospice.github.io/legal/techwithjohann/#data-deletion` | `https://johannhospice.github.io/techwithjohann-legal/#data-deletion` | Johann, ou la session Création avec son accord |
| Enable Banking, application « Fortuna (usage personnel) » | Politique de confidentialité | `https://johannhospice.github.io/legal/fortuna/#privacy` | à relire (probablement `…/fortuna-legal/PRIVACY`) | Johann |
| Enable Banking, application « Fortuna (usage personnel) » | Conditions | `https://johannhospice.github.io/legal/fortuna/#terms` | à relire (probablement `…/fortuna-legal/TERMS`) | Johann |

Chemins de menu :

- Meta : [developers.facebook.com/apps](https://developers.facebook.com/apps) › Tech with Johann › Paramètres de l'app › Général : « URL de la politique de confidentialité » et « URL des instructions de suppression des données ».
- Enable Banking : [enablebanking.com/cp/applications](https://enablebanking.com/cp/applications) › Fortuna (usage personnel) : champs politique de confidentialité et conditions. Ils ne sont pas contrôlés en mode restreint.

Aucun autre organisme n'a reçu d'URL de ces dépôts : Kairos reste en mode test Google, sans page déclarée ; les connecteurs crypto de Fortuna (clés d'API) n'en demandent pas.

## Modifier une politique

1. Modifier la source :
   - Johann | Tech : `CREATION/docs/legal/politique-confidentialite-outil-dm.md`, puis reporter le texte dans `techwithjohann/index.html` (sans la section « Hébergement », réservée à Johann) ;
   - Fortuna : `fortuna/index.html` directement, versions française et anglaise.
2. Changer la date « Dernière mise à jour » et « Last updated ».
3. Garder les ancres du tableau ci-dessus : des services les citent.
4. Pousser sur `main`, puis contrôler que chaque URL répond 200 et que les ancres existent.

Tant que `techwithjohann-legal` n'est pas une redirection, Meta lit encore sa copie : y reporter le même texte. Une fois les anciens dépôts transformés en redirections, ce dépôt est le seul endroit à modifier.

## Transition

`techwithjohann-legal` et `fortuna-legal` restent en ligne tant qu'un service les déclare. Ordre :

1. Les services passent aux adresses de ce dépôt (tableau ci-dessus).
2. Les anciens dépôts deviennent des pages de redirection vers ce dépôt. Pour Meta, seulement après le changement d'adresse : son robot pourrait ne pas suivre la redirection et juger la politique absente.
3. Suppression des anciens dépôts : seulement quand plus aucun service ne les cite, et avec l'accord explicite de Johann.

Domaine : la racine `johannhospice.github.io` est servie par le dépôt `johannhospice.github.io`. Une balise de vérification de domaine (Meta ou autre) va dans l'`index.html` de ce dépôt-là, pas ici.
