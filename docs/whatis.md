# Qu'est-ce que Git ?

## Installation
1. Suivre ce [lien](https://git-scm.com/downloads)
2. Télécharger et installer la version pour votre Système d'opération

Note: Pour la section de PATH, choisir l'option recommandé. Pour les autres configuration, l'option souhaitable est déjà sélectionné.

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

L'utilisation de git permet une tonne d'avantage lors du développement logiciel. Contrairement à ce que l'on croit son utilisation est beaucoup plus large, on peut l'utiliser dans toute sorte de travaux coopératif. En effet, Git n'est pas lier à un type de fichier et permet le versionnement de toute sorte de fichier. La mise en place de git est vraiment simple et permet d'avoir un source singuliaire de vérité pour le stockage de donnée. Plus souvent qu'autrement, je vais même utiliser git dans mes projets solo, car cela me permet de garder une trace de mon travail et d'y enmagasiner mes différentes versions. Cela permet d'y revenir facilement, de transférer facilement mon travail sur plusieurs ordinateurs, consulter rapidement le project sur le repository en ligne, etc.

Parcontre, il faut garder quelques aspects à l'esprit. Git n'est pas fait pour faire le suivi sur les fichiers binaires ou encodés. Ce qui veut dire que git ne va pas ouvrir vos fichiers pdf pour observer les différences, il va simplement l'ouvrir en format texte. Les fichiers binaires peuvent être enmagasinés sur git, mais vous ne pourrez pas profiter des avantages de git comme le controle par ligne et le suivi de changement sur eux. Ceci dit, il faut également garder à l'esprit que les hébergeurs donnent une taille limite aux projets créer sur leur plateforme et cela peut vous limitez dans le type de donnée mis dans votre repository git. (Pour Github, on parle de 500mb total pour les repository privées d'un utilisateur gratuit.)


TLDR : 
- Avantage : 
    - Controle par ligne
    - Travail collaboratif / séparation du travail
    - Ideal pour le code et les fichiers contenant du texte (lisible dans bloc note)
    - Garder toutes les états d'un travail
    - Retour en arrière
- Inconvénients : 
    - Fichiers binaires n'ont pas n'ont pas tous les avantages de git
    - Espace en ligne limité ou payant

***
## Les fournisseurs

Les fournisseurs de Git viennent tous avec un série de fonctionnalité qui leur est propre. Que ça soit des intégrations avec des outils externes, un écosystème complet de développement, des outils simplifier de développement continue, le suivi des bugs, etc. Afin de justifier son existence, chaqu'un est unique en son genre et vient avec sa suite d'avantage et d'inconvénient. Je ne ferai pas ici une liste exostive de tous les fournisseurs, car il en existe plus d'une vingtaine. Je vais seulement parler rapidement de ceux qui sont les plus connu et populaire. (À noter, ils sont simplement en ordre alphabétique)

### Azure DevOps

Azure DevOps est la plateforme git de développeur poussé par Microsoft. En plus de contenir toutes les fonctionnalités classiques d'un fournisseur git, cette plateforme permet de gérer l'intégration et le développement continue sur des services infonuagiques, le contrôle et le suivi des effectifs sur un projet, des outils de déploiement de tests et le storage d'artéfactes permettant le déploiement.

### Bitbucket

Bitbucket est la plateforme git qui est promu par Atlassian. Cela lui permet d'avoir des intégrations simple avec les autres services de la compagnie qui sont des quasi-incontournable du marché(Jira et confluence). Regroupant plus de 5 millions d'utilisateurs, Bitbucket est très utilisé dans l'industrie.

### GitHub

Contant plus de 31 millions d'utilisateurs, GitHub est de loin le plus gros fournisseur de git. Depuis 2018, GitHub est devenu une des subsidiaires de Microsoft. La constante croissante popularité de ce fournisseur vient de la quantité faramineuse de project Open Source qui y ont vu et y voit le jour. Plus souvent qu'autrement, si quelqu'un vous donne un lien de git, ce sera sur cette plateforme. Sur cette plateforme, il y a un certain aspect social permettant de participé à des projets et en récolter les retours. Beaucoup de développeur inclus leur profil GitHub sur leur CV afin de montrer leur implication dans le monde du Open Source.

### GitLab

Le nombre d'utilisateur de GitLab est un mystère et le service n'appartient pas à une des compagnies les plus grosses du monde entier. Qu'est-ce qui fait de ce service l'un des plus populaire et utilisé du marché? Dans ses débuts, GitLab établit que ce sera beaucoup plus qu'un simple service de Git. Dans les années qui suivent, la plateforme intègre des outils qui permettent de facilité le développement et la mise en production. GitLab est la première plateforme à faire cela. Une des caractéristique qui fait que GitLab est unique des 3 autres est que sont code est Open Source. Cela permet donc a qui que ce soit (presque) de se créer son propre serveur de GitLab.

Par Samuel Leclerc
