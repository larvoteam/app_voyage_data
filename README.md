# Données de lieux — Mundoo

Lieux (manger, dormir, visiter) servis à l'appli **Mundoo**, rangés par pays puis en carrés de 0,1°.

- Servi par raw.githubusercontent.com (GitHub Pages ne déploie plus au-delà de 100 000 fichiers ; il garde une ancienne version pour les anciennes versions de l’appli).
- `v2/index.json` : liste des pays (date de mise à jour, nombre de lieux, sources, zones de 5° où le pays a des lieux), colonnes
- `v2/<pays>/index.json` : carrés du pays et nombre de lieux de chacun (`fr`, `de`, `es`…)
- `v2/<pays>/c/<lat>_<lon>.json` : lieux d'un carré (clé = coordonnées × 10, arrondies vers le bas)

Chaque pays a sa propre date : quand un pays est mis à jour, l'appli ne retélécharge que ses carrés. (Format `v1`, une seule liste pour tout le monde, retiré en version 0.29.0 de l'appli.)

Fabriqué avec `tools/places/` (dépôt de l'appli) à partir de :

- **OpenStreetMap** — © contributeurs OpenStreetMap, base de données sous licence [ODbL](https://opendatacommons.org/licenses/odbl/). Ce jeu de données dérivé est lui aussi diffusé sous ODbL.
- **DATAtourisme** — [Licence Ouverte 2.0](https://www.etalab.gouv.fr/licence-ouverte-open-licence/) (data.gouv.fr).

Couverture actuelle : France entière (métropole, Corse et outre-mer ; OpenStreetMap + DATAtourisme) ; Espagne, Portugal, Italie (avec Vatican et Saint-Marin), Suisse, Liechtenstein, Autriche, Allemagne, Belgique, Pays-Bas, Luxembourg, Royaume-Uni (avec Man, Jersey, Guernesey), Irlande, Andorre, Monaco, Malte, Danemark (avec les Féroé), Suède, Norvège, Finlande, Islande, Pologne, Tchéquie, Slovaquie, Hongrie, Slovénie, Croatie, Grèce, Chypre, Roumanie, Bulgarie, Serbie, Bosnie-Herzégovine, Monténégro, Macédoine du Nord, Albanie, Kosovo, Estonie, Lettonie, Lituanie, Moldavie, Ukraine, Biélorussie, Turquie et Russie ; hors d’Europe : Nouvelle-Zélande, Australie ; Asie du Sud-Est : Thaïlande, Vietnam, Cambodge, Laos, Malaisie, Singapour, Brunei, Indonésie, Timor oriental, Philippines, Birmanie ; Asie de l’Est : Chine, Hong Kong, Macao, Japon, Corée du Sud, Taïwan, Mongolie ; Asie du Sud : Inde, Népal, Sri Lanka, Maldives, Bhoutan, Bangladesh, Pakistan (noms coréens et kana japonais translittérés ; noms en idéogrammes, thaïs, khmers, lao et birmans laissés dans leur écriture quand aucun nom latin n’existe) (OpenStreetMap ; noms grecs et cyrilliques translittérés quand aucun nom latin n’existe). DATAtourisme non inclus pour la Corse pour l’instant.

Chaque lieu est rangé dans un seul pays (contours Natural Earth) : les extraits de deux pays voisins se chevauchent un peu.
