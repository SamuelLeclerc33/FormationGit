# [Outils graphiques](https://git-scm.com/downloads/guis)

Afin de faciliter, l'utilisation de git, il existe plusieurs outils graphiques. Ceux-ci permettent de contrôler votre git sans passer par les lignes de commande montrée [ici](./whatdoes.md). Ici, je vais vous parler des 2 plus connus ainsi que de celui que j'utilise au quotidien. À noter que je conseille à tous de bien connaître, leurs commandes git, car il n'est pas toujours possible d'installer un outil graphique sur tous les environnements. De plus, aucun de ceux-ci n'est parfait, donc il souvent simple de contourner les problèmes avec une bonne connaissance des commandes.

## [Git Gui (Windows/Mac/Linux)](https://git-scm.com/docs/git-gui)

Je considère que Git Gui est le plus populaire des Gui, car il vient avec l'installation de git et peut être ouvert par la simple commande : 
> git gui

Ce client inclus la grande majorité des fonctionnalités de git. Étant la première interface utilisateur de git, on peut lui attribuer un certain charme. Son apparence transparaît son âge et malgré le fait qu'on retrouve la majorité des fonctionnalités utiles, elles sont presque toutes cachées dans des menus. L'un des avantages de cette interface est qu'on sait exactement les commandes git qui vont être appelé lorsque l'on fait une action.

## [SourceTree (Windows/Mac/Linux)](https://www.sourcetreeapp.com/)

SourceTree est à ma connaissance l'un des clients git les plus utilisés. Il regroupe la majorité des fonctionnalités dans un client avec un visuel moderne. Comme tout outil, il y a une courbe d'apprentissage, mais sa prise en main se fait facilement et les fonctionnalités les plus utiles sont disponibles contextuellement. SourceTree est gratuit à 100% et permet d'accéder à toutes les plateformes git, qu'elle soit publique ou privée.

## [Git Kraken (Windows/Mac/Linux)](https://www.gitkraken.com/)

Git Kraken est selon moi le client Git le plus complet et celui qui est le plus au goût du jour. Il fournit une interface simple, mais qui permet de faire tout ce qu'un développeur a besoin. La version gratuite offre des intégrations avec la plupart des fournisseurs de Git. Par contre, certaines intégrations qui sont principalement reliées au développement en entreprise (Github Entreprise, GitLab Self-Managed, Bitbucket Server et Azure DevOps) sont accessibles pour la modique somme de 49$/an. La plateforme est gratuite avec Github étudiant, ce qui veut dire que si vous avez un compte avec votre adresse courriel de l'ÉTS, vous avez les Git Kraken pro gratuitement!

***
## Mise en garde

L'utilisation d'un client Git facilite beaucoup d'opérations accomplies quotidiennement par un développeur, mais ils ne sont pas magiques. Une mauvaise manipulation dans un client Git peut causer du dommage difficilement réparable sur le répertoire à distance ou en local, cela peut causer la perte de plusieurs heures de travail.
Malgré que les erreurs de manipulation sont toujours réparables, certaines demandent une connaissance approfondie du fonctionnement des lignes de commande qui ne sont pas présentées ici. Certaines opérations comme les "Force push" ou les "Hard reset" sont déconseillées dans les clients Git, car ils peuvent causer ces dommages.