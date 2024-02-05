
<!--v-->
###### UN SITE DE COMMERCE ÉLECTRONIQUE : shopinaka.com
Cette partie décrit l'analyse des besoins effectuée lors du développement d'un site de commerce électronique de vente de livres de cuisine, appelé shopinaka.com.

Ce site se propose de vendre des livres de cuisine couvrant tous les niveaux d'expertise et tous les types de cuisine. Pour se démarquer des sites similaires, shopinaka.com prévoit de recueillir les avis et commentaires de ses clients et d'offrir une fonctionnalité de gestion de listes de cadeaux.

<!--v-->
###### LES ACTEURS
Les six rôles suivants ont été retenus :
- Internaute : une personne qui peut visiter les pages de présentation et faire des recherches.
- Client : une personne s'étant enregistrée et connectée, qui peut passer des commandes et les suivre, créer et gérer des listes de cadeaux, évaluer et commenter des ouvrages.
- Ami : une personne ayant reçu un code personnalisé permettant d'accéder à une liste de cadeaux et de passer commande dans cette liste.
- Éditeur : un employé chargé des descriptions d'ouvrage, de la classification des ouvrages (niveau d'expertise et catégories d'appartenance) et de la validation des commentaires des clients.
- Gestionnaire : un employé chargé de gérer le catalogue et le stock d'ouvrages.
- Administrateur : un employé chargé du bon fonctionnement du site et de sa maintenance.

Les trois premiers rôles relèvent du front office, les trois derniers du back office. Il existe aussi un acteur logiciel, le Système de paiement sécurisé d'un prestataire externe.

<!--v-->
### User Stories pour l'Internaute :
1. **Rechercher des ouvrages :**
   - En tant qu'internaute, je veux pouvoir effectuer une recherche textuelle dans les descriptions des ouvrages afin de trouver rapidement des livres correspondant à mes intérêts.
   - En tant qu'internaute, je souhaite utiliser une recherche avancée pour filtrer les ouvrages par catégories telles que le niveau d'expertise, la catégorie d'ouvrage et la tranche de prix.
   - En tant qu'internaute, je veux avoir la possibilité de rechercher des ouvrages en fonction de leurs caractéristiques, telles que le titre, l'auteur et le numéro ISBN.
   - En tant qu'internaute, je désire effectuer une recherche basée sur la popularité, en triant les résultats en fonction des avis des clients et des ventes réalisées.

   **Acceptance Criteria :**
   - Les résultats de la recherche doivent inclure uniquement les ouvrages disponibles en stock.

<!--v-->
### User Stories pour l'Internaute :
2. **Consulter un ouvrage :**
   - En tant qu'internaute, je veux pouvoir consulter en détail un ouvrage trouvé, y compris voir la photo de la couverture, ses caractéristiques, sa description, les avis des clients et avoir accès aux commentaires.
   - En tant qu'internaute, je souhaite voir clairement si l'ouvrage est actuellement en stock avant de consulter ses détails.

   **Acceptance Criteria :**
   - Les détails de l'ouvrage doivent être présentés de manière claire et conviviale.
   - L'internaute doit avoir la possibilité de naviguer facilement entre les différentes sections des détails de l'ouvrage.

<!--v-->
### User Stories pour le Client :
1. **S'enregistrer :**
   - En tant que futur client, je souhaite pouvoir fournir des informations obligatoires telles que le nom, le prénom, l'adresse, l'e-mail, le login et le mot de passe lors de mon enregistrement.
   - En tant que futur client, je veux avoir la possibilité de fournir des informations facultatives supplémentaires, comme l'âge et le numéro de téléphone, lors de mon enregistrement.

   **Acceptance Criteria :**
   - Le système doit exiger les informations obligatoires pour permettre l'enregistrement du client.
   - Le système doit permettre au client de fournir des informations facultatives lors de l'enregistrement.
<!--v-->
### User Stories pour le Client :
2. **Se connecter :**
   - En tant que client enregistré, je souhaite me connecter en saisissant mon login et mon mot de passe.

   **Acceptance Criteria :**
   - Le système doit vérifier les informations de connexion du client.
   - Le client doit être redirigé vers la page d'accueil après une connexion réussie.

<!--v-->
### User Stories pour le Client :
3. **Sélectionner des ouvrages dans son panier :**
   - En tant que client, je veux pouvoir ajouter des ouvrages à mon panier en les sélectionnant, les supprimer, et ajuster les quantités souhaitées.
   - En tant que client, je veux être informé en temps réel du nombre d'articles dans mon panier et du montant total de ma commande.

   **Acceptance Criteria :**
   - Le système doit permettre au client d'ajouter, supprimer et ajuster la quantité des ouvrages dans son panier.
   - Le client doit voir le nombre d'articles dans son panier et le montant total mis à jour en temps réel.

<!--v-->
### User Stories pour le Client :
4. **Passer une commande :**
   - En tant que client, je veux pouvoir passer une commande en choisissant les modalités de livraison, le type de livraison, le mode de règlement et en saisissant les coordonnées bancaires sur un serveur de paiement sécurisé externe.
   - En tant que client, je veux recevoir une confirmation d'achat en cas de succès de la transaction financière.

   **Acceptance Criteria :**
   - Le système doit guider le client à travers le processus de commande avec des options claires.
   - Le client doit recevoir une confirmation d'achat avec les détails de la commande après un paiement réussi.

<!--v-->
### User Stories pour le Client :
5. **Consulter ses commandes :**
   - En tant que client, je souhaite pouvoir consulter mes commandes en cours ainsi que l'historique de mes commandes déjà livrées.

   **Acceptance Criteria :**
   - Le système doit fournir un historique des commandes avec des détails tels que le statut, les articles commandés, et les dates.

<!--v-->
### User Stories pour le Client :
6. **Créer une liste de cadeaux :**
   - En tant que client, je veux pouvoir transformer le contenu de mon panier en une liste de cadeaux en spécifiant la nature et la date de l'événement, ainsi que les prénoms et adresses e-mail des amis concernés.

   **Acceptance Criteria :**
   - Le système doit permettre au client de spécifier la nature et la date de l'événement pour créer une liste de cadeaux.
   - Des e-mails personnalisés avec des codes doivent être générés et envoyés aux amis associés à la liste.

<!--v-->
### User Stories pour le Client :
7. **Proposer un avis :**
   - En tant que client, je veux avoir la possibilité de donner mon avis en choisissant parmi un ensemble prédéfini d'appréciations.

   **Acceptance Criteria :**
   - Le système doit fournir une liste d'appréciations préétablies parmi lesquelles le client peut choisir.
   - L'avis du client doit être enregistré et associé à l'ouvrage correspondant.

<!--v-->
### User Stories pour le Client :
8. **Proposer un commentaire :**
   - En tant que client, je souhaite pouvoir saisir un commentaire libre de 500 caractères maximum, qui sera enregistré en attente de validation par un éditeur.

   **Acceptance Criteria :**
   - Le système doit permettre au client de saisir un commentaire de 500 caractères maximum.
   - Les commentaires doivent être enregistrés en attente de validation par un éditeur avant d'être affichés publiquement.

<!--v-->
### User Stories pour l'Ami :
1. **Consulter une liste de cadeaux :**
   - En tant qu'ami, je veux pouvoir consulter une liste de cadeaux en m'identifiant avec le code reçu par e-mail.
   - En tant qu'ami, une fois identifié, je souhaite voir la liste des ouvrages sélectionnés qui n'ont pas encore été choisis, avec leurs caractéristiques, y compris les prix.

   **Acceptance Criteria :**
   - L'ami doit être en mesure de se connecter en utilisant le code reçu par e-mail.
   - La liste des cadeaux restants doit afficher clairement les caractéristiques des ouvrages, y compris les prix.

<!--v-->
### User Stories pour l'Ami :
2. **Acheter des cadeaux dans une liste :**
   - En tant qu'ami, je veux pouvoir sélectionner un ou plusieurs ouvrages dans la liste des cadeaux restants.
   - En tant qu'ami, je veux saisir mes coordonnées personnelles comme celles d'un client lors de l'achat.
   - En tant qu'ami, je veux régler mon achat en suivant le même processus que celui des commandes normales.

   **Acceptance Criteria :**
   - L'ami doit avoir la possibilité de sélectionner les ouvrages dans la liste des cadeaux restants.
   - Le processus d'achat doit être identique à celui des commandes normales, y compris le choix des modalités de livraison, le mode de règlement, et la saisie des coordonnées bancaires sur un serveur de paiement sécurisé externe.
   - L'ami doit recevoir une confirmation d'achat après le règlement réussi.

<!--v-->
### User Stories pour l'Éditeur :
1. **Éditer une description d'ouvrage :**
   - En tant qu'éditeur, je veux pouvoir saisir la description textuelle d'un ouvrage.
   - En tant qu'éditeur, je veux pouvoir spécifier le niveau d'expertise de l'ouvrage (débutant, amateur, chef).

   **Acceptance Criteria :**
   - Le système doit permettre à l'éditeur de saisir et enregistrer une description textuelle d'un ouvrage.
   - L'éditeur doit pouvoir spécifier et enregistrer le niveau d'expertise de l'ouvrage.

<!--v-->
### User Stories pour l'Éditeur :
2. **Gérer les catégories d'ouvrages :**
   - En tant qu'éditeur, je veux pouvoir ajouter une nouvelle catégorie d'ouvrages.
   - En tant qu'éditeur, je veux pouvoir modifier les détails d'une catégorie d'ouvrages existante.
   - En tant qu'éditeur, je veux pouvoir supprimer une catégorie d'ouvrages existante.

   **Acceptance Criteria :**
   - Le système doit permettre à l'éditeur d'ajouter une nouvelle catégorie d'ouvrages avec des détails associés.
   - L'éditeur doit pouvoir modifier les détails d'une catégorie d'ouvrages existante.
   - L'éditeur doit pouvoir supprimer une catégorie d'ouvrages existante.

<!--v-->
### User Stories pour l'Éditeur :
3. **Examiner les commentaires en attente de validation :**
   - En tant qu'éditeur, je veux pouvoir afficher la liste des commentaires en attente de validation.
   - En tant qu'éditeur, je veux pouvoir valider un commentaire en attente.
   - En tant qu'éditeur, je veux pouvoir refuser la validation d'un commentaire en attente.

   **Acceptance Criteria :**
   - Le système doit fournir une interface pour que l'éditeur puisse afficher la liste des commentaires en attente.
   - L'éditeur doit avoir la possibilité de valider un commentaire en attente, le rendant visible publiquement.
   - L'éditeur doit avoir la possibilité de refuser la validation d'un commentaire en attente, le maintenant en attente d'autres actions.

<!--v-->
### User Stories pour le Gestionnaire :
1. **Gérer le catalogue :**
   - En tant que gestionnaire, je veux pouvoir ajouter un ouvrage au catalogue en fournissant ses données factuelles (éditeur, nombre de pages, date de parution, etc.).
   - En tant que gestionnaire, je veux pouvoir modifier les détails d'un ouvrage existant dans le catalogue.
   - En tant que gestionnaire, je veux pouvoir supprimer un ouvrage du catalogue.
   - En tant que gestionnaire, je veux pouvoir afficher l'ensemble du catalogue.

   **Acceptance Criteria :**
   - Le système doit permettre au gestionnaire d'ajouter un nouvel ouvrage au catalogue avec toutes les données factuelles requises.
   - Le gestionnaire doit être en mesure de modifier les détails d'un ouvrage existant dans le catalogue.
   - Le gestionnaire doit être capable de supprimer un ouvrage spécifique du catalogue.
   - Le système doit fournir une fonctionnalité permettant au gestionnaire de visualiser l'ensemble du catalogue.

<!--v-->
### User Stories pour l'Éditeur :
2. **Gérer le stock :**
   - En tant que gestionnaire, je veux pouvoir enregistrer une entrée en stock pour un ouvrage spécifique.
   - En tant que gestionnaire, je veux pouvoir enregistrer une sortie exceptionnelle du stock pour un ouvrage donné.
   - En tant que gestionnaire, je veux pouvoir afficher l'état actuel du stock.
   - En tant que gestionnaire, je veux pouvoir rechercher les ouvrages en fonction du niveau de stock.

   **Acceptance Criteria :**
   - Le système doit permettre au gestionnaire d'enregistrer une entrée en stock, y compris les détails de l'ouvrage et la quantité ajoutée.
   - Le gestionnaire doit être capable d'enregistrer une sortie exceptionnelle du stock avec des détails explicatifs.
   - Le système doit fournir une fonctionnalité permettant au gestionnaire de visualiser l'état actuel du stock.
   - Le gestionnaire doit pouvoir rechercher des ouvrages en fonction du niveau de stock.

<!--v-->
### User Stories pour l'Éditeur :
3. **Suivre les ventes :**
   - En tant que gestionnaire, je veux pouvoir déterminer les ventes selon différents critères tels que la période et le niveau de détail.
   
   **Acceptance Criteria :**
   - Le système doit permettre au gestionnaire de générer des rapports de ventes en spécifiant la période souhaitée.
   - Le gestionnaire doit pouvoir choisir le niveau de détail des rapports de ventes, par exemple, par ouvrage ou par catégorie.

<!--v-->
### User Stories pour l'Administrateur :
1. **Maintenir le site :**
   - En tant qu'administrateur, je veux pouvoir gérer les utilisateurs du back office, y compris les éditeurs, les gestionnaires et les autres administrateurs.
   - En tant qu'administrateur, je veux pouvoir gérer les clients en ayant la capacité de les ajouter, les modifier ou les supprimer.
   
   **Acceptance Criteria :**
   - Le système doit fournir une interface d'administration permettant à l'administrateur de gérer les utilisateurs du back office, y compris l'ajout, la modification et la suppression.
   - L'administrateur doit pouvoir gérer les clients, avec des fonctionnalités telles que l'ajout, la modification et la suppression.
