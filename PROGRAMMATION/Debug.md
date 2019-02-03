<h5 style="text-align: center"> PROGRAMMATION </h5>

------

## **Debug**

------

### 

- Méthode **`fprint`**
  - `fflush(sdtout)` : permet de vérifier qu’un `printf` s’est exécuté
- Débugger : **`gdb`** 
  - `gcc` **`-g`** `-o file file.c`
  - **`gdb`** `file` (exécutable) (sans paramètre)
    - **`run`** `<arg>` : exécute avec des arguments
    - **`db`** : affiche toutes les valeurs des paramètres
    - **`bt`** : affiche où le programme s’est arrêté
    - **`fr 1`** : se place dans la frame/fonction 1 (nombre affiché à coté de `#` dans `bt`)
    - **`l`** : affiche le code autour de la frame
    - **`p var`** : affiche la valeur de la variable `var`
    - **`b file:5`** ou **`b file:func`** : place un point d’arrêt à la ligne (ex : 5) ou à la fonction (ex : func) (`file` est par ex `fichier.c`) (relancer le programme après)
      - `continue` : repart après un point d’arrêt
      - `info breakpoints` : liste des points d’arrêts
      - `delete num_pt` : supprime le point d’arrêt numéro `num_pt`
    - **`set variable nom=expr`** : modifie la valeur de la variable `nom`
    - **`step <arg>`** : descendre dans le corps de la fonction appelée
    - **`next <arg>`** : exécute la fonction complètement
    - **`finish`** : finit l’exécution la fonction
    - **`watch var`** : permet de vérifier qu’une variable a été modifiée
  - **`gdb attach PID`** : se connecter sur un programme créé par un autre programme, en spécifiant le PID du programme à connecter

------

<table width="90%">
<tr>
<td style="width: 30%; text-align: left; background:transparent; border:0;">Langage C</td>
<td style="width: 30%; text-align: center; background:transparent; border:0;">Alexis Bagarre</td>
<td style="width: 30%; text-align: right; background:transparent; border:0;">T1 - 2018 / 2019</td>
</tr>
</table>