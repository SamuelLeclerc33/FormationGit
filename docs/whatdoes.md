# Fonctionalité de base

Ici, nous allons parler des commandes principal de git. Il en existe bien d'autre, mais ce guide non exaustif est ce qui est nécessaire de savoir selon moi. Pour plus d'info cliquer [ici](https://git-scm.com/docs).

## Commandes simple

1. [Config](https://git-scm.com/docs/git-config)

   La commande config a beaucoup d'utilité, mais elle est sur cette liste pour seulement une de celle-ci. Config permet de changer le nom et le courriel de l'utilisateur. Cela permet d'identifier la personne qui interagie avec le répertoire.

   > git config --global user.name "John Doe"

   > git config --global user.email johndoe@example.com

2. Init
   
   Pour commencer un nouveau répertoire git, il faut executer une commande Init. Celle-ci est faite seulement une fois par projet. 

   > git init

3. Add

   Permet d'ajouter des changements dans un commit. Pour rendre cela le plus simple possible, on peut simplement ajouter tout ce qui est dans le répertoire en faisant : 
   > git add *
   
   Mise en garde : il se peut que certain document ne doivent pas être partagé. Nous allons parler plus de cela à la prochaine [ici](./professionalUse.md).

4. Commit
   
   Commit permet de sauvegarder l'état de votre répertoire en local. Un commit regroupe des changements et un message qui les expliquent. Plus souvent qu'autrement, nous allons inclure le message directement dans la commande de commit, car cela évite l'apprentissage de d'autres outils de ligne de commande qui peuvent sembler compliqués (voir Vim).

   > git commit -m "Ici on écrit notre message"

5. Clone

   Permet de copie un répertoire dans un fichier à partir d'une origine distante. Dépendement, le service utilisé les requis seront différents, mais habituellement ceux-ci sont bien expliqué sur la plateforme en ligne. Si vous voulez une copie local de ce répertoire, vous pouvez simplement faire : 

   > git clone https://github.com/SamuelLeclerc33/FormationGit.git

6. Remote

   Remote permet de lier votre répertoire local avec une origine distante. Si vous ne compté pas partagé votre projet, cette commande n'est pas nécessaire. Deplus, si vous clonez celui-ci cette commande est déjà faites pour vous!

   > git remote add origin https://github.com/SamuelLeclerc33/FormationGit.git

7. Pull

   Pull permet de rapatrier les changements qui ont été fait sur votre branche à distance. Si vous avez des changements en cours qui ne sont pas sur l'orgine, cette commande pourrait ne pas fonctionner et vous suggérer des alternatives.

   > git pull

8. Push

   Push permet d'envoyer tous les commits que vous avez fait en local afin de les rendre accessible au gens qui ont accès à votre répertoire à distance. Vous ne pourrez pas push s'il y a des changements sur le repertoire que vous n'avez pas en local. Pour ce faire, il vous faudra merge les changements puis push. 

   > git push

9. Checkout

   Dans plusieurs des fonctions suivantes, je parle de branche, c'est ici que ca se passe. Git permet d'avoir plusieurs branches qui sont des versions différentes du même répertoire. Celle-ci commence à un point et quand nous sommes prêt à intégrer le code à une autre branch, nous pouvons les fusionner ensemble. Checkout permet de créer et de changer de branche à volonté. À noter, si la branche existe en local, Checkout va changer à la version local et non celle qui est sur le répertoire distant. Pour ce faire, il va falloir Pull après avoir checkout afin de consulter les changements.

   Pour changer : 
   > git checkout nomdelabranche

   Pour créer : 
   > git checkout -b nomdelanouvellebranche

10. Stash
   
    Stash permet de mettre de côté les changements en cours afin  de revenir au commit précédent. 
    > git stash
 
    Afin de resortir les informations qui ont été mis de coté, on  utilise Pop.
    > git stash pop
 
    Si vous décidé d'avoir beaucoup d'éléments dans votre stash  (ce qui n'est pas nécessairement une bonne idée), vous pouvez  pop seulement un éléments spécifique du stash.

11. Merge

    Merge permet de prendre une branch et de l'appliquer sur une la branche courante. S'il y a des conflits entre les 2, des bloques de conflit seront ajoutés directement dans les documents visés.

    > git merge autrebranche

Par Samuel Leclerc
