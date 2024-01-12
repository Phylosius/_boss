# Warchall - Begins
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
