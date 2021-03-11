# Examen 1 FORMATIF
Services Web 420-4A4-VI  
Hiver 2021

## Directives
- Vous avez droit à toutes vos notes et Internet.
- Aucune communication n'est permise (messagerie, courriel, etc). Un élève pris en flagrant délit se verra attribuer la note de 0 pour plagiat. 
- La durée de l'examen est de 1h50.
- Vous devez cloner ce projet et implémenter chacun des points demandés.
- Une fois l'examen terminé, faites un git push de votre projet pour me le remettre.

**hint**  
Oubliez pas de faire un **composer update** avant de commencer!!

-----------------------

## Contexte
Examen formatif allégé dans le but de se préparer à l'examen 1

## Points évalués
----------------------------
### Point #1 - Création de la base de données
- Créer un nouvelle base de données appelée **ServicesWeb_Examen1_formatif**
- Rouler le script du répertoire **ressource/sql** pour créer la table et inclure les données.
  - utilisateurs.sql
- Apporter les modifications nécessaires au code pour accéder à la nouvelle base de données.
----------------------------

### Point #2 - Récupérer le mot de passe d'un utilisateur
- Créer la structure nécessaire pour récupérer le mot de passe d'un utilisateur en spécifiant son courriel (Route, Action, Service et Repository).
- Le courriel doit être spécifié dans la route.
- Ajouter les entrées nécessaire de cette route dans la documentation openAPI. Il y a déjà un fichier de débuté (examen1_servicesweb_v1.yaml).
- La réponse doit être formatée comme suit : 
```
{
    "password": "c8c237fb35ada9fb874829cb342a40fd2ea32dc6d78479221c5ab12e51033a99",
}
```
----------------------------

### Point #3 - Ajout d'un résultat
- Créer la structure nécessaire pour pouvoir ajouter un utilisateur.
- Les informations doivent être spécifié dans le body de la requête.
- Ajouter un message dans un fichier de log nommé **Transaction.log** depuis la classe repository pour indiquer l'ajout de l'utilisateur. Le message doit avoir la structure suivante : 
```
[2021-03-11T10:28:20.287054-05:00] UtilisateurCreateRepository.INFO: Utilisateur ID [901] inséré 
```
- La réponse doit être formatée comme suit : 
```
{
    "message": "L'utilisateur a été ajouté",
    "utilisateurId": 901
}
```
- Le code de statut de la réponse doit être 201.
----------------------------

### Point #4 - Commit final et remise
- Une fois l'examen terminé, faire un dernier commit avec la mention **Commit final**
- Ensuite faire un **git push** pour me remettre l'examen. (Je ne corrigerai rien de plus récent que le commit final)

----------------------------
 
## Bon succès!!




