# Analyse des Habitudes d'Utilisation des Applications Mobiles

## Lien Du Projet
Ce projet a été fait par Viet Anh NGUYEN et Sofia MABROUK


## Contexte et Motivation

Aujourd’hui, nous sommes tous accros à nos smartphones et nous ne sommes pas forcément conscients du temps qu’on passe sur nos applications. À travers nos visualisation, nous analysons de manière détaillée les schémas d'utilisation des applications tout au long de la journée et pendant une durée de 11 mois, d'une personne. Notre objectif n'est pas de stigmatiser l'usage des smartphones, mais plutôt de montrer l'importance d'une utilisation consciente des technologies. En effet, notre but est de responsabiliser les utilisateurs en leur fournissant une vue globale mais bien précise de nos interactions avec les technologies.

## Public Cible
Nous ciblons principalement 3 catégories de personnes:

### Développeurs

Cette visualisation offre aux développeurs une perspective inédite sur la manière dont les utilisateurs interagissent avec une application à différentes heures de la journée. Ces informations peuvent les aider à faire des ajustements de conception visant à optimiser l'expérience utilisateur, répondant ainsi de manière plus précise aux besoins et aux habitudes des utilisateurs.

### Marketing

Du point de vue du marketing, cette analyse peut etre très intéressante. En effet, en comprenant les façons d'utilisation à différentes périodes, les campagnes publicitaires peuvent être ciblées de manière plus efficace. Ce qui aide donc à maximiser l'impact publicitaire en adaptant la diffusion au moment optimal pour atteindre les utilisateurs de manière pertinente.

### Chercheurs en Sciences du Comportement

Dans le domaine de la recherche, notre visualisation peut etre une mine d'informations pour les chercheurs en sciences du comportement. Elles fournissent une exploration approfondie des schémas comportementaux liés au monde du numérique, ouvrant la voie à des études approfondies sur la relation entre les individus et leurs téléphones

## Sources de données choisies

Pour la collecte des données, notre objectif initial était d'extraire nos propres données d'utilisation des applications. Cependant, nous n'avons trouvé aucune application qui permettait d'obtenir des données sur une période d'un an, toutes les applications fournissaient des données depuis le premier jour de téléchargement de ces dernières (donc juste pour le mois de decembre). Face à cette limitation, nous avons fait une recherche sur Google Scholar, chrome et Kaggle.

La recherche a été relativement longue, car nous étions spécifiquement à la recherche de jeux de données couvrant une période prolongée afin d'obtenir une quantité suffisante d'informations. Finalement, nous avons identifié le jeu de données suivant: https://www.kaggle.com/datasets/arul08/mobile-usage-dataset-individual-person/data offrant des données d'utilisation d'applications mobiles d'une personne, étendues sur une période de 7 mois. Cette richesse de données nous a permis de créer des bonnes visualisations et a identifier des patterns interessants. 

## Pretraitement de données et langages utilisés
Pour le prétraitement de données, on a utilisé le langage Python:
""" conda create --name M2_DataViz python=3.8

conda activate M2_DataViz

pip install -r requirements.txt

"""
Nos visualisations ont été crée en JavaScript en utilisant principalement la bibliothèque D3.

## Visualisations
Notre travail comprend quatre visualisations principales qui présentent les données de manière de plus en plus détaillée, allant du plus spécifique au plus général.

### Première visualisation

La première visualisation est un bubblechart (diagramme à bulles) conçu pour illustrer l'évolution temporelle des habitudes d'utilisation des applications mobiles. L'idée de créer ce bubble chart est née après la découverte de la visualisation faite par Mr Nathan YAU : https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/. Cela a attiré notre attention et on a décidé de créer une visualisation similaire pour engager à notre tour les visiteurs. L'objectif principal était de fournir une approche créative et visuelle pour rendre les données temporelles relatives aux habitudes d'utilisation des applications plus attrayantes et compréhensibles. Un autre projet qui nous a inspiré et qui mérite d'etre mentionné, c'est celui de nos collègue, étudiant à Lyon 1 Anthony Bardou, Hugo Polloli, Tristan Syrzisko et Théo Rabut : https://abardou.github.io/viz-habits/#/visualisation. Les données sur lesquelles les visualisations ont été crées ressemble aux notres (données d'utilisation des applications mobiles). On a trouvé cela très intéressant et ça nous a encouragé à ne pas changer d'idée et à continuer à travailler avec ces données pour créer un projet à la hauteur de ces deux traveaux.

La visualisation met en avant différentes types d'applications, représentées par des bulles distinctes. L'animation de la visualisation permet à l'utilisateur d'observer comment l'utilisation des applications évolue au file du temps. Cela offre une perspective dynamique sur la façon dont certaines applications deviennent plus fréquemment utilisées à certains moments de la journée, ainsi que comment les habitudes générales changent au fil du temps qui est affiché sur l'horloge située à gauche du bubblechart. On voit aussi une petite image au dessus de l'horloge qui sert à simplifier la vue de l'utilisateur en fonction du moment de la journée (jour, soir,nuit), offrant une expérience plus conviviale au visiteur. Trois boutons (Fast, Stop et Normal) indiquent des options pour contrôler la vitesse de l'animation et l'arreter pour mieux voir les cluster si necessaire. Cette approche créative permet donc à l'utilisateur de mieux comprendre les schémas et les changements dans l'utilisation des applications au fil du temps. L'utilisation d'une animation facilite la perception des tendances temporelles de manière interactive.

### Deuxième visualisation

La deuxième visualisation, complémentaire à la première, propose une heat map (inspiré du tp 4) illustrant le taux d'utilisation des applications au fil du temps. Mais contaitement au bubblechart, elle ne parvient pas à transmettre l'évolution temporelle des habitudes. Elle intègre un slider qui permet à l'utilisateur d'explorer la visualisation de manière interactive, en offrant une vue détaillée des variations temporelles. Ce slider est également connecté à un barchart, facilitant la détection des pics d'utilisation tout au long de la journée. Grâce à cette fonctionnalité, l'utilisateur peut rapidement identifier les moments où certaines applications sont les plus utilisées. En ajustant le slider, l'utilisateur peut comparer visuellement l'utilisation des applications à différents moments de la journée. Ces deux visualisations ont mis en lumière des patterns interessants, comme le fait que de 7h du matin à 9h le propriétaire des données à tendance à utiliser principalement instagram (probablement dès son reveil) puis il utilise son téléphone pour effectuer des appels de de 9h30 à 10h30 du matin et aussi pendant la pause déjeuné (13h à 14h). Mais les patterns les plus intéressants on les voit la nuit, surtout à partir de 21h. L'utilisateur a tendances à utiliser instagram, whatsApp et le téléphone pour effectuer des appels. Cela nous semble logique puisqu'à cet heure ci, d'habitude, les gens ont tendance à se réposer après une longue journée de travail et scroller sur les réseaux sociaux, ou appeler la famille et les amis.

### Troisième visualisation

Concernant la troisième visualisation, elle se concentre sur une analyse comparative de l'utilisation des applications en semaine par rapport au weekend. Un barchart a été élaboré pour illustrer l'utilisation quotidienne de chaque application, distinguant clairement les jours de semaine des jours du weekend. Un pie chart accompagne le bar chart pour comparer le temps moyen d'utilisation pendant les jours de la semaine et le weekend. Cette visualisation révèle que bien que les temps moyens d'utilisation soient similaires (~300 min) pendant un jour en semaine et un jour du weekend, les préférences d'application diffèrent. En semaine, les utilisateurs privilégient des applications pouvant être interrompues à tout moment (comme Instagram, WhatsApp, YouTube), tandis que le weekend, avec plus de temps disponible, est marqué par l'utilisation d'applications nécessitant une durée plus longue, telles que des jeux ou le visionnage de films sur des plateformes comme Disney Plus.

### Quatrième visualisation

Finalement, comme dernière visualisation on a fait un line chart. Cette visualisation offre une vue générale de la durée d'utilisation des applications sur une période de 7 mois. Quelques observations pertinentes ont été identifiées à partir de ces données. Instagram est l'application la plus utilisée tout au long de la période, suivie dans le classement par WhatsApp, YouTube, et les appels téléphoniques. Un motif intéressant apparaît avec l'utilisation d'applications de jeux, qui connaît un pic pendant les mois de mai et juin, suivi d'une pause jusqu'en septembre, puis un retour sur ces applications. Cela peut être attribué aux vacances d'été ou on préfère plutot profiter du beau temps et de la famille que de jouer au jeux. En revanche, des applications comme Goodreads ou les applications de livraison de repas ne suscitent pas beaucoup d'interet de la part de l'utilisateur. La visualisation est complétée par des fonctionnalités interactives, notamment la mise en évidence des lignes lors du survol, permettant une exploration plus détaillée des schémas d'utilisation.

## Organisation Du Travail
Habitant pas loin l'un de l'autre et ayant fait tous nos projets ensemble, mon binôme et moi avons eu la possibilité de majoritairement travailler en direct, sur place, même pendant les vacances scolaires. Cela nous a permis de discuter et de mettre en oeuvre nos idées en temps réel. Lorsque des idées nouvelles émergent, nous les discutons directement ou utilisons Discord dans l'une ou deux fois ou on n'était pas sur place, pour une communication asynchrone. Chaque fois qu'un membre de l'équipe a une nouvelle idée, on en discute ensemble et elle est intégrée au projet au fur et à mesure de son développement. Cette approche a favorisé une collaboration efficace et une communication fluide tout au long du processus de création de notre projet et surtout nous a fait gagner beaucoup de temps.

## Esquisses
![Première Esquisse](./image/image1.jpg)
![Deuxième Esquisse](./image/image2.jpg)
![Troisième Esquisse](./image/image3.jpg)
![Quatrième Esquisse](./image/image4.jpg)
![Dernière Esquisse](./image/image5.jpg)