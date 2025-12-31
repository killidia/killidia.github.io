+++
title = "Devlog #1 - Villager : le tout, tout début !"
slug = "devlog_1_villager_le_tout_debut"
date = "2023-08-09"

[extra]
toc = true
+++

Chers lecteurs et lectrices,

Dans ce deuxième devlog, je souhaite partager avec vous les prémices de l'idée qui a donné naissance à Villager ainsi que mes premiers pas dans le développement de jeu vidéo.

## 1. Les prémices

### Inspiration 1 : Among Us

La première fois que j'ai pensé à Villager, c'est lors d'une soirée assez frustrante à jouer à Among Us, où j'ai été innocent tout au long de la soirée et où je me faisais éliminer systématiquement dès le début. Je me suis donc dit "et si nous avions un jeu similaire où les innocents pourraient se défendre un peu plus à la manière de Garry's Mod et son excellent mode Murder qui donne un pistolet à un des innocents". Et cette simple idée a été le point de départ de ce qui allait devenir Villager.

### Inspiration 2 : Les Battle Royal

Ma deuxième source d'inspiration majeure pour Villager provient des jeux Battle Royal, avec Fortnite en tête, étant un joueur assidu moi-même. J'ai trouvé l'idée de permettre aux "innocents" de chercher des armes et des artefacts qui seraient éparpillés aléatoirement à la manière d'un Battle Royal pour se défendre contre les "imposteurs" super intéressant et proposeraient un gameplay plus sympa que de faire des quêtes en attendant de se faire éliminer comme sur Among Us (oui, j'ai toujours un peu de haine...).

### Inspiration 3 : Les Loup-Garou de Thiercelieux

Après avoir eu l'idée, après avoir trouvé un début de gameplay sympathique, il me fallait un univers captivant pour que les joueurs puissent se plonger pleinement dans l'expérience du jeu. En tant que grand fan des Loup-Garou de Thiercelieux, au point d'avoir un tatouage représentant l'un des rôles du jeu, j'ai pensé que ce serait une excellente base pour mon projet.

### En résumé

![inspirations](../images/devlog_1/inspirations.png)

En résumé ça donne quoi, Villager est un jeu d'imposteur ou les villageois devront survivre aux loups-garous et les loups-garous devront éliminer tous les villageois avant la fin de la nuit. Les villageois devront se faire confiance entre eux, récupérer des armes pour se défendre ou trouver des artefacts qui représenteront les différents rôles que l'on retrouve dans les loups-garous de thiercelieux comme l'orbe de la voyante, l'épée rouiller du chevalier ou encore l'arc de cupidon. Les Loups-garous devront quant à eux user de ruse et de tromperie pour réussir leur sombre dessein.

Le gameplay sera sublimé par une direction artistique minimaliste, mais super efficace, par une ambiance prenante et légèrement oppressante, ainsi que des fonctionnalités comme le chat vocal de proximité pour des interactions sociale efficace (Bon... sans trop vous spoiler, c'est facile à écrire, mais pas facile à faire !!) !

Il m'aura fallu quelques mois pour en arriver là et ce n'était que le tout début du projet. Après avoir posé un premier gameplay sur "papier" je me suis naturellement dit qu'il fallait que je développe un prototype afin d'expérimenter et de vérifier que mon idée était viable. C'est le moment de faire les premiers choix techniques !

## 2. Premier choix technique : Le moteur

### Ureal Engine vs Unity

![ue-vs-unity](../images/devlog_1/ue-vs-unity.png)

En m'engageant dans le domaine du jeu vidéo, je ne voulais pas juste sortir mon jeu pour combler une simple frustration, mais je voulais vraiment en profiter pour en apprendre un maximum sur le développement de jeu vidéo. Pour cela, j'étais à la recherche d'un moteur de jeu qui me permettrait d'explorer en profondeur les différentes couches de la création de jeux, des mécanismes de base jusqu'aux aspects avancés. C'est ainsi que j'ai exclu dès le départ des géants comme Unreal Engine et Unity, qui, bien qu'ils offrent des fonctionnalités puissantes, demandent des licences coûteuses pour la commercialisation. 

### Godot ?

![godot](../images/devlog_1/godot.png)

Après avoir écarté UE et Unity, je me suis penché sur d'autres options open source. Bien que Godot soit un excellent moteur, il ne répondait pas à mon premier critère : la possibilité d'apprendre en partant de presque zéro. De plus, au moment de mon choix, Godot avait encore des gros problèmes de performances, ce qui constituait un élément rédhibitoire pour moi.

### Le langage Rust

En tant que développeur, le choix du langage de programmation est essentiel pour se sentir à l'aise et productif. Pour ma part, Rust est mon langage préféré **DE TOUS LES TEMPS !!!!!!** je me calme... Il offre un équilibre parfait entre performance, sécurité et ergonomie, il possède beaucoup de fonctionnalité pratique et un peu overkill, son écosystème est très vaste et les personnes qui le peuplent sont incroyablement gentils et intelligents. J'avais donc pour objectif de monter en compétences sur Rust tout en développant des jeux, et cela a grandement influencé mon choix de moteur de jeu.

### Le moteur Bevy

![bevy-game-engine](../images/devlog_1/bevy_logo_dark.png)

C'est alors que j'ai découvert Bevy, une véritable perle rare répondant à tous mes critères et bien plus encore. Tout d'abord, Bevy est un moteur de jeu open source, ce qui signifie que je peux accéder à son code source et explorer en profondeur son fonctionnement interne, ce qui est crucial pour mon apprentissage.

En outre, Bevy se démarque par ses performances grâce à sa conception basée sur le design pattern ECS (Entity-Component-System), le moteur gère efficacement les entités et les composants, optimisant ainsi le rendu et le traitement des données, ce qui est essentiel pour créer des jeux fluides et réactifs (mais on y reviendra plus en détail prochainement). 

Choisir Bevy me permettait également de m'impliquer dans son développement. Le moteur étant en cours de développement actif, j'avais la possibilité de contribuer à son évolution, ce qui représentait une chance inestimable pour approfondir mes connaissances et partager ma passion avec la communauté Bevy.

En conclusion, en choisissant Bevy, j'ai trouvé le moteur de jeu idéal pour réaliser mon projet tout en apprenant un maximum de choses dans le développement de jeu vidéo. Grâce à sa gratuité, son statut open source, sa performance, son design pattern ECS et son implémentation en Rust, Bevy réunit tous les éléments clés qui ont guidé mon choix.

![work hard](https://media.giphy.com/media/3o6Ei2yv8fqpR3nJG8/giphy.gif)

Le moteur de jeu choisi, il est grand temps de commencer le développement du premier prototype, mais nous verront ça dans le prochain devlog qui y sera consacré et de toutes les galères que j'ai pu rencontrer pendant ce processus ! Je tiens également à préciser qu'à partir de maintenant les devlogs seront un peu plus techniques.

Merci d'avoir pris le temps de me lire !

A la prochaine,

Dylan.