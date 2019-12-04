# La biométrie humaine
## Guyliann Engels, Raphael Conotte & Philippe Grosjean

## Avant-propos

Ce projet porte sur la biométrie humaine. Ce dernier est un projet qui va évoluer avec votre progression dans les différents modules. Pour ce faire, suivez avec attention les attendus pour chaque module. 

Il est possible que ce document évolue au cours du temps. N'hésitez pas à aller vérifier le lien suivant afin de voir les modifications dans les consignes : <https://github.com/BioDataScience-Course/sdd1_biometry>

## Module 2 : Workflow en biologie : comparaison R et Word _versus_ R et R Markdown

Exercice du cours de [Science des Données Biologiques I de l'Université de Mons, module 02](http://biodatascience-course.sciviews.org/sdd-umons/integration-des-graphiques-dans-un-rapport-r-markdown.html#a-vous-de-jouer-4).

### Objectif

- Réaliser l'intérêt de R Markdown pour écrire des documents scientifiques de manière à ce qu'ils soient reproductibles et faciles à mettre à jour.

### Procédure

Vous êtes dans la peau d'un biologiste qui analyse des données de biométrie humaine. Vous avez à votre disposition deux jeux de données répartis en deux fichiers, disponibles à partir du sous-dossier `data` de ce projet.

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


#### Analyse de `biometry_2014.xlsx`

- Utilisez ce jeu de données afin de réaliser un graphique de type nuage de points (choisissez-en un qui vous parait pertinent). Pour cela, créez un script R `biometry_graphe.R` dans un sous-dossier `R`.

- Incorporez ensuite le graphique généré dans un rapport sous Microsoft Word (fichier nommé `biometry_word.docx` et placé dans le sous-dossier `analysis`). Structurez votre rapport avec les différentes sections de la rédaction scientifique (introduction, but, matériel et méthodes, résultats, discussion et conclusions). Ajoutez une courte phrase relative à chaque section pour donner un peu de contenu à votre rapport, sans plus. Le graphique est à incorporer dans la section "résultats". Des explications détaillées sur la rédaction scientifique se trouvent dans l’[annexe ](http://biodatascience-course.sciviews.org/sdd-umons/redaction-scientifique.html) dédiée à cette dernière.

- Réalisez ensuite le même rapport mais dans un document R Markdown (format .Rmd). Pour cela, complétez le document `biometry.Rmd` mis à votre disposition dans le sous-dossier `analysis` avec les différentes sections propre à un rapport scientifique. Copiez-y le texte que vous avez écrit précédemment, et utilisez le formattage propre à markdown. Incorporez-y également le graphique de type nuage de point dans la partie "résultats". Pour cela, copiez le code R issu du script `biometry_graphe.R` dans un chunks permettant de lire les données, et ensuite de réaliser le graphique.

- Compilez votre rapport R Markdown en trois formats différents : "HTML", "PDF" et "Word". Examinez le résultat, et comparez en particulier les deux version Word de votre rapport.


#### Nouvelles données `biometry_2016.xlsx`

Après avoir réalisé vos deux débuts de rapports, vous recevez des chercheurs de nouvelles données se trouvant dans le dossier `data` qui se nomme `biometry_2016.xlsx`

- Actualisez votre rapport sous Microsoft Word avec ces nouvelles données. Vous devez bien évidemment actualiser le graphique. Actualisez revient donc à remplacer le graphique ancien et plus à jour par un nouveau graphique mis à jour.

- Faites de même pour votre rapport sous R Markdown.

#### Comparaison des deux méthodes

A la suite de vos analyses, répondez aux questions ci-dessous pour cadrer votre réflexion sur le workflow et la recherche reproductible.

Utilisez un fichier Markdown (`.md`) pour y consigner vos réponses et placez-le dans votre projet RStudio. Nommez ce fichier `workflow.Rmd`

- Quel workflow vous semble le plus simple à l'utilisation, et pourquoi ?

- Comparez la façon dont les graphiques sont gérés dans les deux cas.

- Quel workflow vous semble le plus pertinent lorsque les données arrivent progressivement ?

- Quel workflow vous semble le plus simple et le plus approprié lorsque plusieurs personnes collaborent pour rédiger un rapport ? 


### Bilan

Lors de cet exercice comparatif, vous avez eu l'occasion d'utiliser deux workfow différents :

- Une version relativement classique en biologie, basé sur Microsoft Word pour la rédaction,
- Une version utilisant R, R Markdown et RStudio.

Vous avez pu constater les avantages du workflow basé sur R Markdown pour pouvoir reproduire, corriger et/ou amender une analyse. **Ces outils sont des éléments de base constitutifs d'un système qui permet d'analyser des données de manière moderne, rigoureuse, vérifiable et partageable.** Les avantages vous paraissent sans doute minimes sur un petit example simpliste comme celui-ci, mais imaginez une étude plus large qui traite des données volumineuses avec des dizaines de graphiques réalisés par plusieurs personnes différentes au sein de l'équipe...

### Etat de progression 

A la fin de ce module, vous devez avoir 

- un script R nommé `biometry_graphe.R` qui comprend vos premiers graphique que vous utiliserez dans le document `biometry_word.docx` (dans le dossier `analysis`)

- un fichier au format .doc ou .docx nommé `biometry_word.docx` (dans le dossier `analysis`) comprend le nuage de point le plus à jour.

- un fichier au format .Rmd nommé `biometry.Rmd` (dans le dossier `analysis`) qui comprend le nuage de point le plus à jour.

- un fichier au format .md nommé `workflow.md` (dans le dossier `analysis`) qui comprend votre comparaison des workflows.

## Module 3 et 4 : descriptions graphiques

### Objectif

- Compléter votre fichier `biometry.Rmd` (dans le dossier `analysis`) avec des graphiques pertinents et intéressants qui décrivent les données. 

### Etat de progression 

A la fin de ces modules, vous devez avoir différents graphiques dans la section résultat de votre rapport `biometry.Rmd` (dans le dossier `analysis`) qui vont décrire les données. Votre rapport doit comprendre au moins 3 graphiques différents. Ces graphiques doivent être explicité dans votre rapport. 

## Module 5

### Objectifs

- Remanier le tableaux de données afin de proposer des tableaux résumant les données

### Etat de progression 

A la fin de ce module, vous devez proposer au moins 2 tableaux résumant les données mis à votre disposition dans la section résultat de votre rapport `biometry.Rmd` (dans le dossier `analysis`). Chaque tableau doit être explicité dnas le rapport

## Module 6

### Objectifs

- acquérir et traiter des données collectées.

### Acquérir des données

Vous avez réalisé un protocole d'acquisition des données et vous avez complété un tableau de données avec ces métadonnées. Une fois ces données collectées, vous allez entamé une rapport structuré se nommant `biometry2019.Rmd`

### Etat de progression 

A la fin de ce module, vous devez avoir :

- un fichier `biometry2019.Rmd` (dans le dossier `analysis`) structuré avec les sections habituelles d'un rapport scientifique (introduction, but, matériels et métodes, résultats, discussion, conclusions). 

- un script R nommé `biometry2019_importation.R` afin de réaliser l'importation et la sauvegarde des données en local.

- sur base des données que vous avez collecté, vous devez vous fixer une question de recherche ciblée que vous préciserez dans la section but de votre rapport. 

- Votre protocole d'acquisition des données doit être explicité dans la section matériels et méthodes

## Module 8

### Objectif 

- Utiliser le test chi^2 pour analyser vos données. 

### Etat de progression 

A la fin de ce module, vous devez avoir 

- un fichier `biometry2019.Rmd` 
    + une section introduction qui décrit vos données
    + une section but qui explicite la question que vous vous posez
    + une section M&M qui explicite votre protocole d'échantillonage 
    + une section résultats qui comprend au moins 3 graphiques pertinents et 2 tableaux pertinents
    + une section discussion vide pour le moment 
    + une section conclusion vide pour le moment



