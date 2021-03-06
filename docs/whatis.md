# Qu'est-ce que Git ?

## Installation
1. Suivre ce [lien](https://git-scm.com/downloads)
2. Télécharger et installer la version pour votre système d'opération

Note: Pour la section de PATH, choisir l'option recommandée. Pour les autres configurations, l'option souhaitable est déjà sélectionnée.

***
## Invention

Une rapide histoire de Git
Comme de nombreuses choses extraordinaires de la vie, Git est né avec une dose de destruction créative et de controverse houleuse. Le noyau Linux est un projet libre de grande envergure. Pour la plus grande partie de sa vie (1991–2002), les modifications étaient transmises sous forme de patchs et d’archives de fichiers. En 2002, le projet du noyau Linux commença à utiliser un DVCS propriétaire appelé BitKeeper.

En 2005, les relations entre la communauté développant le noyau Linux et la société en charge du développement de BitKeeper furent rompues, et le statut de gratuité de l’outil fut révoqué. Cela poussa la communauté du développement de Linux (et plus particulièrement Linus Torvalds, le créateur de Linux) à développer son propre outil en se basant sur les leçons apprises lors de l’utilisation de BitKeeper. Certains des objectifs du nouveau système étaient les suivants :

- vitesse ;

- conception simple ;

- support pour les développements non linéaires (milliers de branches parallèles) ;

- complètement distribué ;

- capacité à gérer efficacement des projets d’envergure tels que le noyau Linux (vitesse et compacité des données).

Depuis sa naissance en 2005, Git a évolué et mûri pour être facile à utiliser tout en conservant ses qualités initiales. Il est incroyablement rapide, il est très efficace pour de grands projets et il a un incroyable système de branches pour des développements non linéaires. 

([Source](https://git-scm.com/book/fr/v2/D%C3%A9marrage-rapide-Une-rapide-histoire-de-Git))

***
## Ce que c'est git pour moi

L'utilisation de git permet une tonne d'avantages lors du développement logiciel. Contrairement à ce que l'on croit, son utilisation est beaucoup plus large, on peut l'utiliser dans toute sorte de travaux coopératifs. En effet, Git n'est pas lié à un type de fichier et permet de versionner toute sorte de fichiers. La mise en place de git est vraiment simple et permet d'avoir une source singulière de vérité pour le stockage de donnée. La plupart du temps, je vais utiliser git pour mes projets solo, car cela me permet de garder une trace de mon travail et d'y emmagasiner mes différentes versions. Cela permet d'y revenir facilement, de transférer facilement mon travail sur plusieurs ordinateurs, consulter rapidement le projet sur le répertoire en ligne, etc.

Par contre, il faut garder quelques aspects à l'esprit. Git n'est pas fait pour faire le suivi sur les fichiers binaires ou encodés. Ce qui veut dire que git ne va pas ouvrir vos fichiers PDF pour observer les différences, il va simplement l'ouvrir en format texte. Les fichiers binaires peuvent être emmagasinés sur git, mais vous ne pourrez pas profiter des avantages de git comme le contrôle par ligne et le suivi de changement sur eux. Ceci dit, il faut également garder à l'esprit que les hébergeurs donnent une taille limite aux projets créer sur leur plateforme et cela peut vous limitez dans le type de donnée mis dans votre répertoire git. (Pour Github, on parle de 500Mb totaux pour les répertoires privés d'un utilisateur gratuit.)


TLDR : 
- Avantage : 
    - Contrôle par ligne
    - Travail collaboratif / séparation du travail
    - Idéal pour le code et les fichiers contenant du texte (lisible dans bloc-notes)
    - Garder tous les états d'un travail
    - Retour en arrière
- Inconvénients : 
    - Fichiers binaires n'ont pas n'ont pas tous les avantages de git
    - Espace en ligne limité ou payant

***
## Les fournisseurs

Les fournisseurs de Git viennent tous avec une série de fonctionnalité qui leur est propre. Que ça soit des intégrations avec des outils externes, un écosystème complet de développement, des outils simplifiés de développement continu, le suivi des bogues, etc. Afin de justifier son existence, chacun est unique en son genre et vient avec sa suite d'avantages et d'inconvénients. Je ne ferai pas ici une liste exhaustive de tous les fournisseurs, car il en existe plus d'une vingtaine. Je vais seulement aborder les plus populaires. (À noter, ils sont simplement en ordre alphabétique)

### Azure DevOps

Azure DevOps est la plateforme git de développeur poussé par Microsoft. En plus de contenir toutes les fonctionnalités classiques d'un fournisseur git, cette plateforme permet de gérer l'intégration et le développement continue sur des services infonuagiques, le contrôle et le suivi des effectifs sur un projet, des outils de déploiement de tests et l’entreposage d'artefacts permettant le déploiement.

### Bitbucket

Bitbucket est la plateforme git qui est promu par Atlassian. Cela lui permet d'avoir des intégrations simples avec les autres services de la compagnie qui sont des quasi incontournables du marché(Jira et confluence). Regroupant plus de 5 millions d'utilisateurs, Bitbucket est très utilisé dans l'industrie.

### GitHub

Contant plus de 31 millions d'utilisateurs, GitHub est de loin le plus gros fournisseur de git. Depuis 2018, GitHub est devenu une des subsidiaires de Microsoft. La constante croissante popularité de ce fournisseur vient de la quantité faramineuse de projets Open Source qui y ont vu et y voient le jour. La plupart du temps, si quelqu'un vous donne un lien git, ce sera sur cette plateforme. On y retrouve un certain aspect social permettant de participer à des projets et en récolter les retours. Beaucoup de développeurs incluent leur profil GitHub sur leur CV afin de montrer leur implication dans le monde de l’Open Source.

### GitLab

Le nombre d'utilisateurs de GitLab est un mystère et le service n'appartient pas à une des compagnies les plus grosses du monde entier. Qu'est-ce qui fait de ce service l'un des plus populaires et utilisés du marché? Dans ses débuts, GitLab établit que ce sera beaucoup plus qu'un simple service de Git. Dans les années qui suivent, la plateforme intègre des outils qui permettent de faciliter le développement et la mise en production. GitLab est la première plateforme à faire cela. Une des caractéristiques qui fait que GitLab est unique des 3 autres est que son code est Open Source. Cela permet donc à qui que ce soit (presque) de se créer son propre serveur de GitLab.

Par Samuel Leclerc
