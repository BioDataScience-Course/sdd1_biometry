# Workflow en biologie : Comparaison R et Word vs R et R Markdown
## Guyliann Engels, Raphael Conotte & Philippe Grosjean

Exercice du cours de [Science des Données Biologiques I de l'Université de Mons, module 02](http://biodatascience-course.sciviews.org/sdd-umons/integration-des-graphiques-dans-un-rapport-r-markdown.html#a-vous-de-jouer-4).

## Objectif

- Réaliser l'intérêt de R Markdown pour écrire des documents scientifiques de manière à ce qu'ils soient reproductibles et faciles à mettre à jour.

## Procédure

Vous êtes dans la peau d'un biologiste qui analyse des données de biométrie humaine. Vous avez à votre disposition deux jeux de données, répartis en deux fichiers, disponibles à partir du sous-dossier `data` de ce projet.

- `biometry_2014.xlsx`
- `biometry_2016.xlsx`

Ces fichiers comprennent 7 variables :

- gender : homme (H) ou femme (F)
- db : date de naissance
- yb : année de naissance
- weight : masse en kg
- height : taille en cm
- wrist : circomférence du poignet en mm
- measurement_date : année de la prise de mesure


### Analyse de `biometry_2014.xlsx`

- Utilisez ce jeu de données afin de réaliser un graphique de type nuage de points. 
Pour cela, créez un script R `biometry_graphe.R` dans un sous-dossier `R`.

- Incorporez ensuite le graphique généré dans un rapport sous Microsoft Word (fichier nommé `biometry.docx` et placé dans le sous-dossier `analysis`). Structurez votre rapport avec les différentes sections de la rédaction scientifique (introduction, but, matériel et méthodes, résultats, discussion et conclusions).

Des explications détaillées sur la rédaction scientifique se trouvent dans l’[annexe ](http://biodatascience-course.sciviews.org/sdd-umons/redaction-scientifique.html) dédiée à cette dernière.

- Réaliser ensuite la meme chose mais dans un document R Markdown. Pour cela, complétez le document `biometry.Rmd` mis a votre disposition dans le sous-dossier `analysis` avec les différentes sections propre à un rapport scientifique. Incorporez-y également le graphique de type nuage de point dans la partie résultats. Pour cela, copier le code R utilisé précédemmant dans un chunks permettant de lire les données, et ensuite de réaliser le graphique.

### Nouvelles données `biometry_2016.xlsx`

Considérez ce fichier comme des données supplémentaires acquises après la rédaction du rapport `biometry.docx`.

- Actualisez votre rapport sous Microsoft Word avec ces nouvelles données. Vous devez bien évidemment actualiser le graphique.

- Faites de même pour votre rapport sous R Markdown.

### Comparaison des deux méthodes

A la suite de vos analyses, répondez aux questions ci-dessous pour cadrer votre réflexion sur le workflow et la recherche reproductible.

Utilisez un fichier Markdown (`.md`) pour y consigner vos réponses et placez-le dans votre projet RStudio.

- Quel workflow vous semble le plus simple à l'utilisation ?

- Comparez la façon dont les graphiques sont gérés dans les deux cas.

- Quel workflow vous semble le plus pertinent lorsque les données arrivent progressivement ?

- Quel workflow vous semble le plus simple et le plus approprié lorsque plusieurs personnes collaborent pour rédiger un rapport ? 


## Bilan

Lors de cet exercice comparatif, vous avez eu l'occasion d'utiliser deux workfow différents :

- Une version relativement classique en biologie, basé sur certains outils Microsoft Office,
- Une version utilisant R, R Markdown et RStudio

Vous avez pu constater les avantages du workflow basé sur R Markdown pour pouvoir reproduire, corriger et/ou amender une analyse. **Ces outils sont des éléments de base constitutifs d'un système qui permet d'analyser des données de manière moderne, rigoureuse, vérifiable et partageable.** Les avantages vous paraissent sans doute minimes sur un petit example simpliste comme celui-ci, mais imaginez une étude plus large qui traite des données volumineuses avec des dizaines de graphiques réalisés par plusieurs personnes différentes au sein de l'équipe...
