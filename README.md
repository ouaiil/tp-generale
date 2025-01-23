Sécurité des Architectures Micro-services avec OAuth2, OpenID Connect, JWT, et Keycloak

Objectif:

L'objectif de cette activité est de mettre en œuvre une solution de sécurisation pour une architecture micro-services en utilisant Keycloak pour gérer l'authentification et l'autorisation. Nous utiliserons les protocoles OAuth2 et OpenID Connect pour sécuriser les communications entre les services, en particulier via l'utilisation de JWT (JSON Web Tokens).
Partie 1 : Configuration de Keycloak

1. Télécharger Keycloak 19

    Objectif : Télécharger et installer Keycloak version 19 pour commencer à gérer l'authentification des utilisateurs et des clients.
    Action : Allez sur le site officiel de Keycloak (Télécharger Keycloak) et téléchargez la version 19.

2. Démarrer Keycloak

    Objectif : Lancer Keycloak pour commencer à gérer les micro-services.
    Action : Dans le terminal, décompressez l'archive et lancez Keycloak avec la commande suivante :

    ./bin/standalone.sh -Djboss.http.port=8080

    Vous pouvez maintenant accéder à l'interface d'administration de Keycloak via http://localhost:8080.

3. Créer un Compte Administrateur

    Objectif : Créer un compte admin pour pouvoir configurer Keycloak.
    Action : Lors du premier démarrage de Keycloak, vous serez invité à créer un compte administrateur. Suivez les instructions pour créer un utilisateur admin.

4. Créer une Realm

    Objectif : Créer un Realm pour gérer les utilisateurs, rôles et clients dans Keycloak.
    Action : Une fois connecté à l'interface d'administration, créez une nouvelle Realm via l'option "Add Realm".

5. Créer un Client à Sécuriser

    Objectif : Créer un client (par exemple, une application web ou une API) que vous souhaitez sécuriser avec Keycloak.
    Action : Dans votre Realm, créez un client en spécifiant les paramètres nécessaires (type d'application, redirections, etc.).

6. Créer des Utilisateurs

    Objectif : Créer des utilisateurs dans le Realm pour les authentifier.
    Action : Allez dans la section "Users" et ajoutez plusieurs utilisateurs avec des informations d'identification spécifiques.

7. Créer des Rôles

    Objectif : Créer des rôles afin de contrôler l'accès aux différents services et ressources.
    Action : Dans la section "Roles", créez des rôles (par exemple : Admin, User) et configurez-les selon vos besoins.

8. Affecter des Rôles aux Utilisateurs

    Objectif : Assigner des rôles aux utilisateurs afin de leur attribuer des droits d'accès spécifiques.
    Action : Dans la section "Users", choisissez un utilisateur et attribuez-lui un ou plusieurs rôles préalablement créés.

9. Tester l'Authentification avec Postman

    Tester l'authentification avec le mot de passe
    
    Analyser les contenus des deux JWT (Access Token et Refresh Token)
    
    Tester l'authentification avec le Refresh Token
    
    Tester l'authentification avec Client ID et Client Secret
    
    Changer les paramètres des Tokens (Access Token et Refresh Token)
    
    Sécurisation d'un Micro-Service Spring avec Keycloak
    
    Sécurisation d'un Frontend Angular avec Keycloak

10. Technologies Utilisées

    Keycloak : Système de gestion de l'authentification et de l'autorisation.
    
    OAuth2 et OpenID Connect : Protocoles utilisés pour sécuriser l'accès aux services.
    
    JWT (JSON Web Tokens) : Format de token utilisé pour les échanges sécurisés entre les services.
    
    Spring Boot : Framework utilisé pour créer les micro-services backend.
    
    Angular : Framework utilisé pour le frontend.
    
![1](https://github.com/user-attachments/assets/c45f75cd-4c42-4c20-a1b3-b2739dd3100c)

![2](https://github.com/user-attachments/assets/edf6d2ef-d7e6-48fd-b9d7-abfb93df1f38)

![3](https://github.com/user-attachments/assets/2285fc07-7177-4201-9c8e-89b3fba5ab8c)

![4](https://github.com/user-attachments/assets/0efa297e-c79a-4500-89ce-327c46e429fc)

![5](https://github.com/user-attachments/assets/eb30bd2a-0ecb-4a8b-97aa-171f552dbc2b)

![6](https://github.com/user-attachments/assets/afe9eb3d-378f-4683-89b5-c5b8b3507ad2)

![7](https://github.com/user-attachments/assets/80c88dd7-f7d8-4fe9-8e63-ba90f9d9af38)

![8](https://github.com/user-attachments/assets/97c191a5-8594-4490-b7c6-f75becb8a064)

![9](https://github.com/user-attachments/assets/de9f6a19-bc86-4af2-a3ab-eb99a1658523)

![10](https://github.com/user-attachments/assets/a531d5d7-d428-4ac5-9f97-b6527e06bed3)

![11](https://github.com/user-attachments/assets/55adc09b-247a-485e-976e-e84723cb7728)

![12](https://github.com/user-attachments/assets/b00da8d1-1500-4f24-be7b-f56cfcc5b5e5)
