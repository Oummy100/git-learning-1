#Explication des corrections du Module2
##Exercice1
###Les commandes utilisées

Lors de la correction du premier exercie, les commandes utilisées sont les suivantes:

```brew install gh``` :Pour installer l'interface de ligne de commandes github, un outil créé par github qui permet d'utiliser github depuis le terminal sans avoir le besoin d'utiliser le site web
                       ````brew````c'est le gestionnaire de packages macOS, qui permet d'installer des outils logiciels sur les systèmes d'exploitation Apple, macOS ainsi que Linux.
                       ```install```` : Elle dit à hombrew d'installer quelque chose (un outil du choix de l'utilisateur, ici gh)

````brew update```` : Pour chercher une mise à jour disponible de homebrew et mettre à jour si disponible.

````gh --version```` : Pour voir la version de l'interface de ligne de commande GitHub
                     ````gh```` :Qui est l'outil de l'interface de ligne de commande GitHub 
                     ````--version```` :qui dit au programme d'afficher la version

````gh repo create```` : Pour créer un nouveau repo GitHub depuis le terminal. Une fois tapé et entré, le processus de création se lance:

1. Il sera demandé quel type de repo l'on veut:
  - Créer un nouveau repo à partir de zéro
  - Cloner un repo existant
  - Importer un repo    

2. Il sera demandé:
  - Le nom du repo
  - La description (qui est optionnel
  - La visibilité: Public ou Privé
  - Ajouter un README, .gitignore, ou une license

3. Après ````gh```` va:
  - Créer un repo sur GitHub
  - De manière optionnelle, ajouter un remote (origine) dans le repo local
  - De manière optionnelle pusher les commits locaux sur GitHub
  

Remarque: il existe une syntaxe qui permet de faire tout le processus en une seule commande: ````gh repo create MonNouveauRepo --public --source=. --remote=origin --push````


````gh repo create MonNouveauRepo````

          Dit à GitHub CLI de créer un nouveau repo sur GitHub appelé MonNouveauRepo.

```--public````

         - Définit la visibilité du repo comme publique, tout le monde pourra le voir. 
         - L'on pourra aussi utiliser -- private s'il prefère que cela soit cahé.

````--source=.````

         - Utilise le dossier courant (.) comme le repo local qui sera connecté à GitHub.
         - Tous les fichiers dans le dossier feront partie du repo.

````--remote=origin````

         - Ajoute un git remote appelé origin qui pointe vers le nouveau repo GitHub.

         - Cela permettra de pusher et de faire un pull facilement après.

````--push````

         - Va pusher tous les commits locaus dans le repo courant immédiatement vers GitHub

         - Important: Le dossier doit contenir au moins un commit, sinon ça ne marchera pas.
 

````git init```` :Pour initialier un nouveau repo git dans le dossier courant, Une fois la commande tapée:
                 - Elle crée un fichier caché .git dans le dossier qui stocke toutes les historiques des versions, commits et configuration de git
                 - De manière basique, elle change le dossier en un repo git

````mkdir```` : Pour creéer un nouveau dossier

`````cd`````: Pour aller d'un repertoir à un autre

`````git add .````` : Pour ajouter tous le contenu du fichier à commiter 

````git commit -m "Message"```` : `````git commit````: crée un commit qui est comme une version enrégistrée d'un projet à un point spécifique dans le temps; ````-m "Message"````: laisse passer un message qui decrit le commit

````touch````: Pour créer un nouveau fichier

````gh repo list NomUtilisateur --limit 100```` : ````gh repo list```` lite les repo GitHub, ````NomUtilisateur```` ajoute le nom de l'utisateur dont les repo seront affichés, ````--limit 100```` limite la liste à 100 repo

````gh repo clone MonRepo```` : Pour cloner (copier) le repo GitHub vers la machine locale 
````rm -r```` : Pour supprimer un dossier anisi que tout son contenu
````ls```` :Pour lister le contenu d'un repertoir
```echo "TexteAAjouter" >> NomDuFichier.txt```` : Pour ajouter du texte dans un fichier
````cat```` :Pour afficher le contenu d'un fichier 
````nano````/````vim```` : Deux commandes differentes utilisées pour éditer du texte mais à la difference de vim, nano presente une extensibilité limitée
```ls -b```` : Pour lister les fichié d'un repertoir tout en affichant des code d'echappement s'ls contiennent des charactères inhabituels comme les espaces, tabs, emojis, les lettres avce accent, etc

````git push```` : Pour pousser un repo local git vers un reférentiel distant 
