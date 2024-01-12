# Warchall - Begins
Tout les solution ont été remplacé par des suite d'astérix (ex: *****)
## Level 00
- Affichage du répertoire courant.

    entré : 
    ```bash
    pwd
    ```
    sortie :
    ```
    /home/user/duduk
    ```
- Affichage des fichiers et dossier du répertoire courant.
    
    entré : 
    ```bash
    ls
    ```
    sortie :
    ```
    WELCOME.md  level  www  www_access.log  www_error.log
    ```
- Affichage du contenu de WELCOME.md .
    Le fichier contient un message de bienvenue et l'emplacement des levels.

    ```
    You will find the solution to each level in
    /home/level
    or
    /home/user/yournick/level
    ```
- Changement du répertoire courant vers : **/home/level**

    entré :
    ```bash
    cd /home/level
    ```
- Affichage du contenu du répertoire courant

    entré :
    ```bash
    ls
    ```

    sortie :
    ```bash
    00_welcome      04_kwisatz          10_choose_your_path   15_live_rfi  special
    01_choice_tree  05_privacy          11_choose_your_path2  20_live_rce
    02              07_tropical_fruits  12_pytong             level01
    03              08_sshz             14_live_fi            matrixman
    ```
- Entrer dans le répertoire : **00_welcome**
    
    ```bash
    cd 00_welcome
    ```
- Affichage du contenu du répertoire courant : **/home/level**

    entré :
    ```sh
    ls
    ```

    sortie :
    ```sh
    README.md
    ```
- Affichage du contenu de **README.md**

    entré :
    ```sh
    cat README.md
    ```

    IL y a une ligne qui donne la solution :
    ```
    Oh .... and your solution to level0 is: "*********" without the quotes.
    ```
- Retour au répertoire parent : /home/level 
    
    entré :
    ```sh
    cd ..
    ```
> [!NOTE]
> La solution est dans : /home/level/00_welcome/README.md

## Level 01
- Entrer dans le répertoire du niveau: **/home/level/01_choice_tree**

    entré :
    ```sh
    cd /home/level/01_choice_tree
    ```
- Affichage du contenu du répeertoire courant : **/home/level/01_choice_tree**

    entré :
    ```sh
    ls
    ```
    sortie :
    ```
    README.md  blue  green  red
    ```
- Lecture de : **README.md**

    entré :
    ```sh
    cat README.md
    ```
    sortie :
    ```
    Hello Hacker,

    You do not need to read this.
    good luck!

    ```
- Affiche récursive du contenu du répertoire courant : **/home/level/01_choice_tree**

    entré :
    ```sh
    ls -R
    ```
    sortie :
    ```
    .:
    README.md  blue  green  red

    ./blue:
    hats

    ./blue/hats:
    black  grey  white

    ./blue/hats/black:
    jedi.md

    ./blue/hats/black/jedi.md:
    sith.md

    ./blue/hats/black/jedi.md/sith.md:
    PATH.path

    ./blue/hats/grey:
    solution

    ./blue/hats/grey/solution:
    patience

    ./blue/hats/grey/solution/patience:
    SOLUTION.txt

    ./blue/hats/white:
    README.EXE

    ./green:
    README.md

    ./red:
    you.die
    ```

    > [!NOTE]
    > On abouti à _5 autres fichiers_ (autre que README.md du répertoire : **/home/level/01_choice_tree**)
    - on trouve les fichiers suivants :

    ```sh
    # PATH.path
    ./blue/hats/black/jedi.md/sith.md/PATH.path
    # SOLUTION.txt
    ./blue/hats/grey/solution/patience/SOLUTION.txt
    # README.EXE
    ./blue/hats/white/README.EXE
    # README.md
    ./green/README.md
    # you.die
    ./red/you.die
    ```
- Affichage du contenu des fichiers trouvés
    ----
    #### PATH.path
    entré : 
    ```sh
    cat ./blue/hats/black/jedi.md/sith.md/PATH.path
     ```
    sortie : 
    ```
    cat: ./blue/hats/black/jedi.md/sith.md/PATH.path: Permission denied
    ```
    ----
    #### SOLUTION.txt
    entré : 
    ```sh
    cat ./blue/hats/grey/solution/patience/SOLUTION.txt
     ```
    sortie : 
    ```
    This was just a little warmup.
    The solution to level 1 is "********" without the quotes.
    ```
    ----
    > [!NOTE]
    > Après avoir régarder une à une le contenu de tous les fichiers trouvés, on constate que **la solution est dans le fichiers SOLUTION.txt** (./blue/hats/grey/solution/patience/SOLUTION.txt
    )
- Retour au répertoire parent : **/home/level** 
    
    entré :
    ```sh
    cd ..
    ```
> [!NOTE]
> La solution est dans : /home/level/01_choice_tree/blue/hats/grey/solution/patience/SOLUTION.txt

## Level 02
- Entrer dans le répertoire du niveau: **/home/level/02**

    entré :
    ```sh
    cd /home/level/02
    ```
- Affichage du contenu du répeertoire courant : **/home/level/02**

    entré :
    ```sh
    ls
    ```
    sortie :
    ```
    documents  photos
    ```
    . On trouve deux dossiers.
- Affichage récursive du contenu (element caché comprise) du répertoire courant : **/home/level/02**

    entré :
    ```sh
    ls -R -al
    ```
    sortie (résumé) :
    on trouve 3 fichiers
    ```sh
    # thumbnails
    ./photos/thumbnails
    # letter.txt
    ./documents/letter.txt
    # .solution
    ./.porb/.solution
    ```
- Vérification du contenu des fichiers trouvés
    
    Après avoir regarder une à une le contenu des trois fichiers trouvés, on constate que __la solution est dans : *.porb/.solution*__

    entré :
    ```sh
    cat .porb/.solution
    ```
    sortie :
    ```
    The solution is **************

    ```
- Retour au répertoire parent : **/home/level** 
    
    entré :
    ```sh
    cd ..
    ```
> [!NOTE]
>La solution est dans : **.porb/.solution**

## Level 03
- Entrer dans le répertoire du niveau: **/home/level/03**

    entré :
    ```sh
    cd /home/level/03
    ```
- Affichage du contenu du répertoire courant (element caché compris) : **/home/level/03**

    entré :
    ```sh
    ls -a
    ```
    sortie :
    ```
    .  ..  .bash_history  .local
    ```
- Affichage du contenu de **.bash_history**

    entré :
    ```sh
    cat .bash_history
    ```
    sortie (résumé): **on remarque une ligne qui donne la solution**
    ```
    The solution to SSH3 is: ****************
    ```
- Retour au répertoire parent : **/home/level** 
    
    entré :
    ```sh
    cd ..
    ```
> [!NOTE]
>La solution est dans : **./.bash_history**

# Level 04
- Entrer dans le répertoire du niveau: **/home/level/04_kwisatz**

    entré :
    ```sh
    cd /home/level/04_kwisatz
    ```
- Affichage du contenu du répertoire courant (element caché compris) : **/home/level/04_kwisatz**

    entré :
    ```sh
    ls -a
    ```
    sortie :
    ```
    README.nfo
    ```
- Affichage du contenu de **README.nfo**

    entré :
    ```sh
    cat README.nfo
    ```
    sortie :
    ```
    Look in your ~

    ```
- Déplacement vers mon ~ (répertoire personnel) avec la commande:
    ```
    cd
    ```
- Affichage du contenu de mon répertoire personnel

    entré :
    ```sh
    ls
    ```
    sortie :
    ```
    WELCOME.md  level  www  www_access.log  www_error.log
    ```
- Entrer dans le répertoire **level** et affichage de son contenu

    entré :
    ```sh
    ~$ cd level
    ~$ ls
    ```
    sortie :
    ```
    04_kwisatz
    ```
- Entrer dans le répertoire **04_kwisatz**
eet affichage de son contenu

    entré :
    ```sh
    ~$ cd 04_kwisatz
    ~$ ls
    ```
    sortie :
    ```
    README.txt  README2.md
    ```
- Affichage du contenu de **README.txt**

    entré :
    ```sh
    cat README.txt
    ```
    sortie :
    ```
    Dear Future Hacker,

    I wrote you an important message in README2.md
    Please act accordingly.

    The WarChall Staff 2023!

    (c) 2011 kwisatz
    ```
    >[!NOTE]
    > On nous dit de voir le contenu de __README2.md__
 - Affichage du contenu de __README2.md__
    - affichage avec : _cat_
    
        entré :
        ```sh
        cat README2.md
        ```
        sortie :
        ```
        cat: README2.md: Permission denied
        ```
        . On n'a pas la permission pour la lecture du fichier

    - ajout du droit de lecture du fichier __README2.md__
        ```sh
        chmod +r README2.md
        ```

    - affichage avec _cat_
        entré :
        ```sh
        cat README2.md
        ```
        résumé de la sortie : __on a une ligne qui donne la solution__ du niveau (flag):
        ```
        Your flag is: "***********************" without the quotes.
        ```
- Retour au répertoire parent : **/home/level** 
    
    entré :
    ```sh
    cd ..
    ```
> [!NOTE]
>La solution est dans : **~/level/04_kwisatz/README2.md** mais il faut d'abord ajouter le droit de lecture pour ce fichier.

    
