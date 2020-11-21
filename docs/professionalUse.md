# Utilisation dans le monde professionnel
Utilisé par toutes les entreprises qui doivent partagés/entreposer du code. Git est devenu un standard pour le travail collaboratif impliquant du code. Ici, je vais présenté une méthode de travail qui est répendu dans l'industrie pour compartimenter et facilité le travail d'équipe et diminuer les conflits.

## [Git flow](https://datasift.github.io/gitflow/IntroducingGitFlow.html)

Git flow donne des définitions à chaque branche afin d'organiser l'information dans le répertoire en ligne. Dans Git flow, il y a 5 types de branche que nous expliquerons ici.

- master
 
  Est la version fonctionnel de l'application. Souvent, master va représenter le produit qui est sur les environnement de production. On va placer des Tags sur différents commits de master afin de définir les versions. La branche master est unique.

- develop
  
  Cette branche représente l'état de développement du projet. C'est à partir de cette branche que les développeur qui font des nouvelles fonctionnalités devraient commencer. develop est également unique, mais peut porter un autre nom.

- features

  Ces branches vont portez des noms suivant le format "features/nomDeLaBranche". Ce sont sur ces branches que les développeurs vont faire leurs changements. Typiquement, elles commencent à partir de develop et sont mergé dans celle-ci. Habituellement, les branches feature ne devrait pas éditer le même code, car cela pourra créer des conflits et la résolution de conflits est l'une des pratiques que l'on essaie d'éviter, car elle amène des bugs.

- release

  Cette branche contient le code qui est en test. C'est l'étape avant que le code se retrouve sur master et soit sur les environnement de production. Il est commun de faire des changement sur cette branche afin de réparer des bugs simple trouvé par les tests QA. Si les changements sont trop important, la release ne devrait pas passer vers master et retourner en développement. Si un changement est fait sur cette branche, celui-ci devrait se refléter sur develop également.

- hotfixes

  Ces branches vont portez des noms suivant le format "hotfixes/nomDeLaBranche". Typiquement, les hotfixes commencent de la branche master et sont mergé dans master et dans develop. Celles-ci contiennent les changements qui doivent être faits sur la branche master lorsque l'on trouve des bugs en production.

En plus de définir des rôles pour chaque type de branche, Git flow spécifie que lorsque l'on veut merger des branches ensembles, la source doit être à jour avec la destination. Pour se faire, il faut que la branche de source se [rebase](https://git-scm.com/docs/git-rebase) sur la destination avant que celle-ci soit mergé ensemble.

Du visuel : 

![visuel](https://dzone.com/storage/temp/12887668-1577951038067.png "visuel")

Pour plus d'information, cliquer sur le titre pour consulter 