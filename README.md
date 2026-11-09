# Données de lieux — Mundoo

Lieux (manger, dormir, visiter) servis à l'appli **Mundoo**, rangés en carrés de 0,1°.

- `v1/index.json` : liste des carrés, colonnes, sources, date de mise à jour
- `v1/c/<lat>_<lon>.json` : lieux d'un carré

Fabriqué avec `tools/places/` (dépôt de l'appli) à partir de :

- **OpenStreetMap** — © contributeurs OpenStreetMap, base de données sous licence [ODbL](https://opendatacommons.org/licenses/odbl/). Ce jeu de données dérivé est lui aussi diffusé sous ODbL.
- **DATAtourisme** — [Licence Ouverte 2.0](https://www.etalab.gouv.fr/licence-ouverte-open-licence/) (data.gouv.fr).

Couverture actuelle : France entière (métropole, Corse et outre-mer ; OpenStreetMap + DATAtourisme), Luxembourg, Andorre, Monaco et Malte (OpenStreetMap). DATAtourisme non inclus pour la Corse pour l’instant.

Chaque lieu est rangé dans un seul pays (contours Natural Earth) : les extraits de deux pays voisins se chevauchent un peu.
