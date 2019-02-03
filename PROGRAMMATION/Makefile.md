<h5 style="text-align: center"> PROGRAMMATION </h5>

------

## **Makefile**

------

### Vocabulaire

- Cible : fichier exécutable
- Dépendances : fichier dont dépend la cible, exemple le fichier `.c`
- 



---

### Création du Make

- Création des `.o` : `gcc -c file.c`
- Création de l’exécutable : `gcc -o exec file.o file2.o file3.o`
- `nm` : regarde le contenu :
  - d’une bibliothèque `.a` / `.so`
  - d’un fichier objet `.o`
  - d’un exécutable
- `lld` : liste les dépendances de bibliothèque

------

<table width="90%">
<tr>
<td style="width: 30%; text-align: left; background:transparent; border:0;">Matière</td>
<td style="width: 30%; text-align: center; background:transparent; border:0;">Alexis Bagarre</td>
<td style="width: 30%; text-align: right; background:transparent; border:0;">T1 - 2018 / 2019</td>
</tr>
</table>