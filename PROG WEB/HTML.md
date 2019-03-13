<h5 style="text-align: center"> PROGRAMMATION WEB </h5>

------

## **HTML**

------

### Écriture du texte

- En C : table ASCII
- En HTML : besoin de plus de caractères (accents, caractères d’autres langues...)
- Utilisation de la table Unicode

---

### Ressources HTML

- Arbre : tous les nœuds ont des étiquettes et des attributs (clé~i~ = valeur~i~)
- Utilisation de marqueurs :
  - Début : `<a>`
  - Fin : `</a>`
  - Si pas d’enfants : `<a/>` (en XML)
  - Toujours une seule racine (marqueur qui englobe tout le code)
- Attributs : `<a cle1="valeur1" cle2="valeur2">...</a>`
- Pas de balises qui se chevauchent
- Special entities : `&___;` (ex: symbole **<** $\rightarrow$ `&lt;`, symbole **&** $\rightarrow$ `&amp;`)

---

### Structure HTML

```html
<doctype html>
<html>
    <head>
    </head>
    <body>
    </body>
</html>
```

- `head` : stock les métadonnées (utiles pour les ressources, ne s’affiche pas à l’écran)
- `body` : ressources



- Balises
  - metadata content (dans le `head`)
    - `<title>` : titre de l’onglet
    - `<meta>` (ex: `charset="utf-8"`, auteurs, date)
    - `<script>` : insérer du code JavaScript
    - `<style>` : pour le CSS
  - body content
    - sectionning content (ex: sommaire, chapitres) $\rightarrow$ *on n’en met jamais trop*
      - `<section>`
      - `<article>`
      - `<aside>`
      - `<header>` : délimite une zone d’en-tête
      - `<footer>` : pied de page
      - `<nav>` : délimite la zone du sommaire
    - flow content (ex: blocs mais pas dans le sommaire)
      - `<p>` : paragraphe
      - `<a>` : lien hypertexte
      - `<ul>` ou `<ol>` puis `<li>` : listes à puce
      - `<table>` puis `<row>` puis `<tr>` puis `<td>` : tableaux
      - `<div>` : balise de regroupement quelconque
      - `<h1>` $\rightarrow$ `<h6>` : titres
    - phrasing content (ex: phrases, mots)
      - `<strong>`
      - `<span>`
      - `<br>` : retour à la ligne (déconseillé)
    - binary content (ex: ce qui n’est pas du texte, images, sons)
      - `<img>` : image
      - `<video>`
      - `<audio>`





------

<table width="90%">
<tr>
<td style="width: 30%; text-align: left; background:transparent; border:0;">Informatique</td>
<td style="width: 30%; text-align: center; background:transparent; border:0;">Alexis Bagarre</td>
<td style="width: 30%; text-align: right; background:transparent; border:0;">T1 - 2018 / 2019</td>
</tr>
</table>