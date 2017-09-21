---
date: 2017-07-11
location: Paris
attendees:
- Joël Gombin
- Thimy Kieu
- Thomas Parisot
---

# Entretien avec Joël Gombin

## Présentation

Joël accompagne les structures publiques et privées à l'_ouverture des données_ ainsi qu'à leur _réutilisation_ sous forme de :

1. Conseil ;
2. Formation (culture, technique — avec [R](https://www.r-project.org/) notamment) ;
3. Médiation (la CAF de Paris par exemple).

[Datactivist](http://datactivi.st/) réalise l'évaluation indépendante des engagements de la France au sein de l'[Open Government Partnership](https://www.opengovpartnership.org/) (_OGP_), mais aussi des engagements de la _Ville de Paris_ ([lire sa candidature à l'OGP](https://www.opengovpartnership.org/sites/default/files/Paris%20Candidacy%20OGP_0.pdf)).

Joël est spécialisé dans la sociologie électorale quantitative. Pratique qu'il exerce depuis 2005.

> Quand tu ouvres tes données, tu ne sais pas comment elles vont être utilisées.

Enfin, Joël a participé à la création de [DODOData](http://www.dododata.io/) pour aider à **automatiser les demandes** à la [Commission d'Accès aux Documents Administratifs](http://www.cada.fr/) (_CADA_) ainsi que le **retraitement des données**, notamment via l'interconnexion entre les différentes plate-formes de données.

## Thématique • Découverte des données

> Le moteur de recherche est perfectible.

> Je cherche beaucoup de fois le terme [élections](https://www.data.gouv.fr/fr/search/?q=%C3%A9lections) pour trouver des données d'élections. Le bon jeu de données est souvent _noyé_ dans les résultats.

😯 Aucun résultat n'est récent

---

🔍 "[Prénoms](https://www.data.gouv.fr/fr/search/?q=pr%C3%A9noms)"

* 🙂 Il y a 1 jeu de données de l'INSEE
* 🤔 Il y a 50 jeux locaux qui redécoupent ce jeu de l'INSEE

🔍 "[élections présidentielles](https://www.data.gouv.fr/fr/search/?q=%C3%A9lections+pr%C3%A9sidentielles)"

* 🤔 Le classement n'est pas compréhensible
	* Le premier jeu correspond à des _élections municipales_
	* Le quatrième correspond aux _élections européennes_
	* Puis arrivent ensuite des jeux relatifs aux _élections cantonales_ et aux _élections législatives_
	* ❗️Enfin arrive en 8ème position un jeu _mentionnant explicitement_ _élections présidentielles_
* Par contre en commençant à saisir "**e**lections présidentielles" l'auto-complétion indique un résultat potentiel intéressant.
![](search-elections-presidentielles.png)
![](search-élections-presidentielles.png)
* 😕 Les tags n'aident pas à trier dans ce cas de figure
* 😨 Pour trouver un résultat récent (de 2017), le mieux est encore d'utiliser la _recherche Google_ (à requête équivalente)

> D'ailleurs Google m'affiche même le post de blog.

![](google-élections-présidentielles.png)


> Je favorise les jeux de données au format CSV ou Excel, ça va beaucoup plus vite à manipuler.

🤔 La recherche fonctionne uniquement si on cherche le bon mots-clés (qui n'est pas connu à l'avance et qui demande du temps à découvrir car souvent spécifique au vocabulaire des administrations).

---

> Je regarde souvent les derniers jeux de données publiés sur la page d'accueil.

![](latest-datasets.png)

---

> Des fois j'utilise les _thématiques_ mais leur classement fait très _administration publique_

---

> Il n'y a pas d'autres plates-formes qui _aggrègent autant_ de données que data.gouv.fr.

---

❗️ Si une commune renseigne mieux un jeu de métadonnées/tags qu'une administration publique, elle devancera un Ministère par exemple.

😤 C'est problématique car un jeu de données à couverture nationale contenant le même type d'information est _plus important_.

🤔 Sans compter que chaque découpage local contient son lot de colonnes spécifiques et le reformate à sa sauce.

---

👎 Les onglets sont peu visibles.

👎 Les facettes sont peu visibles/lisibles également. De par leur taille et emplacement notamment.

💬 Organiser les résultats de manière moins linéaire peut-être ?

---

🔍 "[élection présidentielle](https://www.data.gouv.fr/fr/search/?q=%C3%A9lection+pr%C3%A9sidentielle)" vs. "[Élection présidentielle Paris](https://www.data.gouv.fr/fr/search/?q=%C3%A9lection+pr%C3%A9sidentielle+paris)"

😤 Même en cherchant sur le nom exact du dataset il n'apparait pas dans les résultats.

😤 "[election présidentielle 2017](https://www.data.gouv.fr/fr/search/?q=Election+pr%C3%A9sidentielle+2017)" ne mène pas à "[Election présidentielle des 23 avril et 7 mai 2017 - Résultats du 2ème tour
](http://www.data.gouv.fr/fr/datasets/election-presidentielle-des-23-avril-et-7-mai-2017-resultats-du-2eme-tour-1/)".

---

🔍 "accidents"

😤 L'autocomplete ne montre que des résultats du département des Vosges.

![](search-accidents-autocomplete.png)

![](search-accidents.png)

🔗 [Accidents de la route](https://www.data.gouv.fr/fr/datasets/accidents-de-la-route/)

---

🔍 "sirene"

![](sirene-autocomplete.png)

😤 L'autocomplete ne donne rien (découpage local), donc on lance la recherche.

![](sirene-search.png)

👍 On a le bon résultat en premier.

## Thématique • Compréhension des données

🔗 [Election présidentielle des 23 avril et 7 mai 2017 - Résultats du 2ème tour](https://www.data.gouv.fr/fr/datasets/resultats-de-lintegralite-des-elections-depuis-2001/)

![](search-intégralité-élections.png)

À propos des métadonnées :

* 😕 Couverture temporelle indique aller jusque 2014 alors qu'en inspectant les données, elle va jusqu'en… 2017
* 😤 La granularité est fausse
* 😤 Il n'y a _que 2 lignes de description_

![](dataset-dates.png)

> D'ailleurs quand je vois XML, dans ma tête je traduis par XL (Excel).

🤔 L'encart _Détails_ n'en contient d'ailleurs pas davantage.

![](dataset-details.png)

> Je sais qu'il y a un guide technique pour utiliser les données mais il n'apparait pas.

💬 Je vais devoir aller le chercher sur le site web du producteur de données.

👎 Il n'y a pas de lien hypertexte pour aller sur le site du producteur depuis le dataset — ni depuis la page de l'organisation.

---

> Une page de dataset me permet de voir de suite les données dont j'ai besoin.

💬 Avoir la **liste des colonnes**, éventuellement les lignes.

---

🔗 [Base Sirene des entreprises et de leurs établissements (SIREN, SIRET)](https://www.data.gouv.fr/fr/datasets/base-sirene-des-entreprises-et-de-leurs-etablissements-siren-siret/)

💬 Ça serait bien de savoir qu'on va télécharger un fichier de 1.4Go de données… (Ressource _Sirene : stock au \<jour\> \<mois\> \<année\>_).


## Thématique • Utilisation des données

> Je peux perdre beaucoup de temps à comprendre les données.

> De manière générale les jeux de données sont très durs à lire.

🔗 [Accidents de la route](https://www.data.gouv.fr/fr/datasets/accidents-de-la-route/)

💬 Le nettoyage de 3 ou 4 fichiers CSV et la lecture de la notice d'utilisation a pris ½ journée à nettoyer et à comprendre.

😤 On a découvert que le champ _adresse postale_ était tronqué sur 20 caractères.

😤 D'autres fois ce même champ contenait des _latitudes_ et _longitudes_.

💬 Certaines informations de compréhension sont présentes dans les discussions. Elles mériteraient d'être mises en valeur.

## Thématique • Contributions

> J'ai 2 comptes mais c'est rare quand je suis connecté : quand je publie des données ou participe à une discussion.

## Conclusion

> Je suis content de voir qu'on s'intéresse à l'aspect UX/UI de data.gouv.fr.

## ROTI • Retour sur le Temps Investi

4
