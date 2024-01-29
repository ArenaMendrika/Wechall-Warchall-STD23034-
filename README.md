# Wechall-Warchall-STD23034-
Examen individuel SYS1


**Première fois sur WeChall ?**
 

 - Initiez votre parcours sur WeChall (https://www.wechall.net/) en cliquant sur le bouton d'inscription situé en haut à droite de la page.
 - Après avoir accompli cette première étape, procédez à la connexion en tant qu'utilisateur, similaire à l'approche sur des plateformes telles que Facebook. Notre défi en cours est dénommé Warchall.
 - Pour aborder ce défi, il est impératif de créer un compte SSH. Considérez cette étape comme l'établissement d'une voie privée sur Internet. Vous serez invité à définir et à confirmer un mot de passe sécurisé en utilisant l'option "(RE)SET your SSH account". C'est à ce moment que la situation devient sérieuse.
 - Finalisez la préparation en ouvrant un terminal. Pour ma part, j'ai utilisé PuTTY, mais vous pouvez également opter pour d'autres clients SSH prenant en charge la connexion à distance à un serveur, tels que Termius, OpenSSH, ou d'autres de votre choix. Assurez-vous de configurer correctement le client SSH pour débuter avec succès le challenge.


**[Training: Warchall - The Beginning](https://www.wechall.net/challenge/warchall/begins/index.php "Training: Warchall - The Beginning")** **Level 0 - 5**
 
 --> LEVEL 0
 
 - **Connexion SSH :** Après avoir saisi votre nom d'utilisateur et votre mot de passe SSH, vous devriez accéder à votre répertoire personnel, généralement représenté par "~".
 - **Exploration initiale :** Utilisez la commande  `ls`  pour examiner les fichiers et répertoires présents dans votre répertoire personnel. Cette commande vous donnera un aperçu des éléments qui vous entourent.
 - **Navigation vers le dossier level :** Puisque les équipes de Warchall indiquent que les solutions se trouvent dans le dossier "/home/level", utilisez la commande `cd /home/level` pour vous déplacer vers ce répertoire spécifique.
 - **Ouverture du dossier "00_welcome" :** Dans level, ouvrez le dossier "00_welcome" en utilisant la commande `cd 00_welcome`. Ceci est nécessaire car nous sommes actuellement au level0, et les solutions peuvent être organisées dans des dossiers spécifiques.
 - **Ouverture du fichier README.md :** Identifiez le fichier README.md en utilisant la commande `ls`. Ensuite, pour lire son contenu, tapez `cat README.md`
 - **Analyse du fichier README.md :**  Lisez attentivement le contenu pour trouver des indices ou des instructions. La solution au level0 est mentionnée à la dernière phrase du fichier.

--> LEVEL 1

 - **Allons dans le dossier 01_choice tree :** Utilisez `cd /home/level/01_choice_tree` pour accéder au dossier du level1.
 - **Explorez le contenu du dossier :** Utilisez `ls` pour voir les fichiers et dossiers dans le dossier 01_choice_tree.
 - **Ouvrez le dossier "blue" :** Comme la solution n'était pas dans README.md, utilisez `cd blue/` pour accéder à ce dossier.
 - **Entrez dans le dossier "hats" :** Utilisez `cd hats/` pour explorer le contenu du dossier hats.
 - **Pénétrez dans le dossier "grey" :** Utilisez `cd grey/` pour accéder à ce dossier.
 - **Trouvez le dossier "solution" :** Utilisez `cd solution/` pour accéder au dossier solution.
 - **Accédez au dossier "patience" :** Utilisez `cd patience/` pour explorer ce dossier.
 - **Ouvrez le fichier SOLUTION.txt :** Utilisez `cat SOLUTION.txt` pour afficher le contenu du fichier SOLUTION.txt et retrouver la solution du level1.

--> LEVEL 2

 - **Entrez dans le dossier 02 :** Utilisez `cd /home/level/02` pour accéder au dossier du level2.
 - **Affichez tous les fichiers, y compris les fichiers cachés :** Utilisez `ls -al` pour afficher tous les fichiers, y compris les fichiers cachés.
 - **Allez dans le dossier caché ".porb" :** Si le dossier caché ".porb" est visible, utilisez `cd .porb` pour y accéder.
 - **Ouvrez le fichier ".solution" :** Utilisez `cat .solution` pour afficher le contenu du fichier ".solution" et accéder à la solution du level2.

--> LEVEL 3

 - **Accédez au dossier 03 :** Utilisez `cd /home/level/03` pour entrer dans le dossier du level3.
 - **Affichez tous les fichiers, y compris les fichiers cachés :** Utilisez `ls -al` pour afficher tous les fichiers, y compris les fichiers cachés.
 - **Ouvrez le fichier .bash_history :** Utilisez `cat .bash_history` pour afficher le contenu du fichier .bash_history et vous pouvez maintenant voir la solution au level3
 
 --> LEVEL 4
 - **Accédez au dossier 04_kwisatz :** Utilisez `cd /home/level/04_kwisatz`.
 - **Regardez les fichiers présents avec ls :** Vous devriez voir un fichier appelé README.nfo.
 - **Le README.nfo indique d'aller dans votre répertoire personnel :** Utilisez `cd ~`.
 - **Entrez dans le dossier "level" :** Utilisez `cd level`.
 - **À l'intérieur du dossier "level", entrez dans "04_kwisatz" :** Utilisez `cd 04_kwisatz`.
 - **Affichez les fichiers présents avec ls :** Vous verrez README.txt.
 - **README.txt conseille d'aller dans README2.md, actuellement inaccessible.**
 - **Vérifiez les droits sur README2.md avec ls -al.**
 - **Ajoutez le droit de lecture pour README2.md avec` chmod +r README2.md`.**
 - **Ouvrez README2.md avec cat README2.md pour accéder à la solution.**

--> LEVEL 5

 - **Entrez dans le dossier 05_privacy :** Utilisez `cd /home/level/05_privacy`.
 - **Vérifiez la présence du fichier README.md avec :** `ls`. Vous devriez voir README.md.
 - **Ouvrez le fichier README.md avec :** `cat README.md` pour accéder à la solution.
