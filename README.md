# Données de lieux — Mundoo

Lieux (manger, dormir, visiter) servis à l'appli **Mundoo**, rangés en carrés de 0,1°.

- `v1/index.json` : liste des carrés, colonnes, sources, date de mise à jour
- `v1/c/<lat>_<lon>.json` : lieux d'un carré

Fabriqué avec `tools/places/` (dépôt de l'appli) à partir de :

- **OpenStreetMap** — © contributeurs OpenStreetMap, base de données sous licence [ODbL](https://opendatacommons.org/licenses/odbl/). Ce jeu de données dérivé est lui aussi diffusé sous ODbL.
- **DATAtourisme** — [Licence Ouverte 2.0](https://www.etalab.gouv.fr/licence-ouverte-open-licence/) (data.gouv.fr).

Couverture actuelle : France entière (métropole, Corse et outre-mer ; OpenStreetMap + DATAtourisme) ; Espagne, Portugal, Italie (avec Vatican et Saint-Marin), Suisse, Liechtenstein, Autriche, Allemagne, Belgique, Pays-Bas, Luxembourg, Royaume-Uni (avec Man, Jersey, Guernesey), Irlande, Andorre, Monaco, Malte, Danemark (avec les Féroé), Suède, Norvège, Finlande, Islande, Pologne, Tchéquie, Slovaquie, Hongrie, Slovénie, Croatie, Grèce, Chypre, Roumanie, Bulgarie, Serbie, Bosnie-Herzégovine, Monténégro, Macédoine du Nord, Albanie, Kosovo, Estonie, Lettonie, Lituanie et Moldavie (OpenStreetMap ; noms grecs et cyrilliques translittérés quand aucun nom latin n’existe). DATAtourisme non inclus pour la Corse pour l’instant.

Chaque lieu est rangé dans un seul pays (contours Natural Earth) : les extraits de deux pays voisins se chevauchent un peu.
