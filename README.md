# PumpFun Paper Trader — vue live

Page statique (aucune librairie externe) qui affiche en direct le portefeuille **papier** (simulation, aucun vrai trade).

- Les données arrivent via [ntfy.sh](https://ntfy.sh) : le watcher publie un instantané toutes les ~20 s sur un topic secret.
- Le topic n'est **pas** dans le dépôt : ouvre la page avec `https://<user>.github.io/<repo>/#<topic>`.
- Au chargement, la page récupère le dernier instantané (10 dernières minutes), puis reste connectée en SSE.
- Quiconque connaît le topic peut lire les données : garde le lien privé.

Données approximatives, aucune garantie.
