<h5 style="text-align: center"> PROGRAMMATION WEB </h5>

------

## **Programmation côté client**

------

### Applications statiques



1. Connexion TCP avec le serveur sur le port 80 (pour HTTP)

   Connexion SSL avec le serveur sur le port 443 (pour HTTPS)

2. Requête HTTP **GET** 

3. Toutes les ressources disponibles sont stockées sur le disque du serveur (ex: dossier `/var/www/`) et recherche du fichier `index.html`

4. Ouverture du fichier `index.html` en RAM par le serveur, ajout des en-têtes (`200 OK`)

5. Envoie les données et ferme la connexion



- Avantages :
  - Léger côté serveur
  - Sécurité (peu de faille car pas d’exécution de code)
  - Simplicité de développement







------

<table width="90%">
<tr>
<td style="width: 30%; text-align: left; background:transparent; border:0;">Informatique</td>
<td style="width: 30%; text-align: center; background:transparent; border:0;">Alexis Bagarre</td>
<td style="width: 30%; text-align: right; background:transparent; border:0;">T1 - 2018 / 2019</td>
</tr>
</table>