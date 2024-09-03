Bonjour,
L'équipe qui travaille sur ce projet est composée de  Youssef Elmelh,  Hicham Skouti, Said .
Nous avons commencé par le prototypage et le maquettage en utilisant Figma. Ensuite, nous sommes passés au développement du frontend, où nous utilisons React.js et CSS pour le design. Pour le backend, nous utilisons Node.js, MongoDB, Express.js, et WebSocket.
Voici les différentes étapes :

## prototypage et du maquettage :
Login / Signup : Page de connexion et d'inscription
Page d'accueil : Affichage général des notes
Page Note : Afficher et gérer une note
Page de réception des notes : Recevoir les notes partagées par d'autres utilisateurs
Page Profil : Gestion du profil utilisateur

## 📄 Frontend : 
### page inscription : 
+ **Formulaire:**
  - ✏️ Nom:
  - ✉️ Email:
  - 🔒 Mot de passe:
  - 🔄 Confirmer le mot de passe:
+ **🔘 Bouton d'inscription** 

### page connexion : 
+ **Formulaire:**
  - ✉️ Email:
  - 🔒 Mot de passe:
+ **🔘 Bouton de connexion** 

### page home :
+ **Header :**
  - logo (lien cliquable)
  - Note reception
  - icons notification (lien cliquable)
      - carte notification  
        - Button accepter 
        - Button supprimer 
  - icon profile (lien cliquable) ==> vers page profile

+ **Sidebar :**
  - list de category des notes creer
  - username d'utilisateur authentifier
  - icons logout 
+ **Contenu :**
  - Button Shared : filtrer les notes partager et non partager 
  - Button New Note
    - Formulaire pop up :
      - title
      - category
      - description 
     -Button add note
  - Carte de note 
    - Icons epingle 
    - Button View (cliquable) ==> vers page Note
+ **Page Note :**
  - carte note : titre + description 
  - Button Share : partager la note avec autre utilisateur 
      - formulaire pop up :
        - username 
        - email 
        - Role 
      - Button share
  - Button Update :
      - formulaire pop up :
        - title 
        - category
        - description 
      -Button update note
  - Button Delete
  - Tables 
      - Option Role : View/Edit
      - Action : 
        - Button Update : update role
        - Button Delete 



   | User      | Email              | Role      | Action     |
   |-----------|--------------------|-----------|------------|
   | john   | john@example.com   |Edite/View |Update/Delete|
   |----       | -----@example.com  | --------- | ----------|

+ **Page Profile :**
  - Button update userInfo:
      - formulaire :
        - username 
        - email
  - Button change password:
      - formulaire :
        - password 
        - confirme password

+ **Note reception :**
  - list des carte de note reçu par autre utilisateur
 

## 📄 Backend : 
### page inscription/connexion: 
  - utilisation fetch API pour l'envoi des donnee
  - 🔒 utilisation de bcrypt pour crpter le Mot de passe
  - 🔄 utilisation validator pour que le mot de passe etre fort:
### page home :
+ **Header :**
  - Utilisation de WebSocket pour la gestion des notifications
  - Recevoir des notifications
  - Cartes de notifications : afficher les notes partagées avec l'utilisateur
+ **Sidebar :**
    - Filtrage des notes par catégories
    - Bouton de déconnexion
+ **Contenu :**
    -  Afficher toutes les notes : récupération des données des notes depuis la base de données
    - Bouton "Shared" : filtrer les notes partagées et non partagées
    - Bouton "New Note": Envoyer les données des notes à la base de données
### Page Note :
    -  Afficher une note : récupération des données de la note depuis la base de données
    - Mettre à jour une note : modifier les données de la note dans la base de données
    - Supprimer une note : supprimer les données de la note dans la base de données
    - Partager une note : partager une note avec d'autres utilisateurs
    - Afficher les données de l'utilisateur avec qui la note a été partagée
    - Gérer les droits d'accès de l'utilisateur qui a reçu la note, gestion du permission de voir ou de modifier la note reçue
### Page Profile :
    - Afficher les données de l'utilisateur
    - Modifier les données de l'utilisateur

### Note reception :
  - Afficher la note avec les droits définis par l'utilisateur qui a partagé la note

+ **test :**
  - Utilisation de Postman pour tester les Api restful 










  















  



