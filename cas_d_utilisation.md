
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
###### **LES CAS D'UTILISATION**

Après discussion entre les porteurs du projet et les développeurs experts en sites marchands, la première liste de cas d'utilisation suivante a été établie en considérant successivement les interactions essentielles initiées par chaque type d'acteur.

<!--v-->
D'accord, voici une version complétée du cas d'utilisation de l'Internaute avec des scénarios détaillés et des conditions spécifiques :

### Cas d'utilisation de l'Internaute :

<!--v-->
#### Acteurs Principaux :
- **Internaute (Utilisateur non enregistré sur le site):** La personne utilisant l'application pour rechercher et consulter des ouvrages.

#### Description :

1. **Rechercher des Ouvrages :**
   - L'application offre aux internautes plusieurs méthodes de recherche.

   **Scénarios :**
   - *Effectuer une Recherche Textuelle dans les Descriptions :* L'internaute peut saisir des mots-clés pour effectuer une recherche textuelle dans les descriptions des ouvrages.
   - *Effectuer une Recherche Avancée par Catégories :* L'internaute peut spécifier le niveau d'expertise, la catégorie d'ouvrage, et une tranche de prix pour affiner sa recherche.
   - *Effectuer une Recherche par les Caractéristiques de l'Ouvrage :* L'internaute peut rechercher des ouvrages par titre, auteur, ou numéro ISBN.
   - *Effectuer une Recherche selon la Popularité :* L'internaute peut trier les résultats par avis des clients et ventes réalisées.

   **Conditions Spécifiques :**
   - Seuls les ouvrages disponibles en stock doivent apparaître dans les listes de résultats.

2. **Consulter un Ouvrage :**
   - L'ouvrage trouvé par l'internaute est présenté en détail avec la photo de sa couverture, ses caractéristiques, sa description, l'avis des clients, et un accès aux commentaires.

   **Scénarios :**
   - *Trouver un Ouvrage :* L'internaute sélectionne un ouvrage dans la liste des résultats de recherche.
   - *Consulter les Détails de l'Ouvrage :* L'internaute accède aux détails complets de l'ouvrage, y compris sa couverture, ses caractéristiques, sa description, l'avis des clients, et un accès aux commentaires.

#### Exigences Préalables :
- Le système doit maintenir une base de données à jour des ouvrages disponibles en stock.
- Les fonctionnalités de recherche doivent être accessibles même aux utilisateurs non enregistrés.

Ce cas d'utilisation détaille comment un Internaute interagit avec le système pour rechercher des ouvrages et consulter les détails d'un ouvrage trouvé. Les scénarios spécifiques fournissent des exemples concrets d'actions que l'Internaute peut entreprendre pour accomplir ces tâches.

<!--v-->
### Cas d'utilisation du Client :
- Acteurs Principaux :
   - **Client (Utilisateur final):** La personne utilisant l'application pour effectuer des actions liées aux ouvrages et aux commandes.
- Description :
   1. S'enregistrer
   2. Se Connecter
   3. Rechercher des Ouvrages et Consulter un Ouvrage
   4. Sélectionner des Ouvrages dans son Panier
   5. Passer une Commande
   6. Consulter ses Commandes
   7. Créer une Liste de Cadeaux
   8. Proposer un Avis et un Commentaire
- Conditions Spécifiques :
   - Le client doit être authentifié pour accéder à certaines fonctionnalités telles que passer une commande, consulter ses commandes, créer une liste de cadeaux, proposer un avis, et proposer un commentaire.

- Exigences Préalables :
   - Le client doit avoir un compte enregistré avec des informations valides.

Ce cas d'utilisation détaille comment un client interagit avec le système pour s'enregistrer, effectuer des recherches, sélectionner des ouvrages, passer des commandes, consulter ses commandes, créer des listes de cadeaux, et proposer des avis et des commentaires. Les scénarios spécifiques fournissent des exemples d'actions que le client peut entreprendre pour accomplir ces tâches.

<!--v-->
### Cas d'utilisation du Client :
1. **S'enregistrer :**
   - Le futur client fournit des informations obligatoires telles que le nom, le prénom, l'adresse, l'e-mail, le login et le mot de passe lors de son enregistrement.
   - Le client peut également fournir des informations facultatives supplémentaires telles que l'âge, le téléphone, etc.

   **Scénarios :**
   - *Fournir des Informations Obligatoires :* Le client remplit le formulaire d'inscription en fournissant toutes les informations obligatoires.
   - *Fournir des Informations Facultatives :* Si le client le souhaite, il peut également ajouter des informations facultatives à son profil.

<!--v-->
### Cas d'utilisation du Client :
2. **Se Connecter :**
   - Le client enregistré se connecte en saisissant son login et son mot de passe.

   **Scénarios :**
   - *Saisir les Identifiants :* Le client entre son login et son mot de passe pour accéder à son compte.

<!--v-->
### Cas d'utilisation du Client :
3. **Rechercher des Ouvrages et Consulter un Ouvrage :**
   - Le client recherche des ouvrages en utilisant différentes méthodes, et peut consulter en détail un ouvrage trouvé.

   **Scénarios :**
   - *Effectuer une Recherche Textuelle :* Le client recherche des ouvrages en utilisant une recherche textuelle dans les descriptions.
   - *Consulter un Ouvrage :* Le client sélectionne un ouvrage trouvé pour voir sa description, ses caractéristiques, les avis des clients, etc.

<!--v-->
### Cas d'utilisation du Client :
4. **Sélectionner des Ouvrages dans son Panier :**
   - Le client peut ajouter, supprimer et ajuster la quantité des ouvrages dans son panier.

   **Scénarios :**
   - *Ajouter des Ouvrages au Panier :* Le client sélectionne des ouvrages et les ajoute à son panier.
   - *Modifier la Quantité d'Ouvrages :* Le client ajuste la quantité d'un ouvrage dans son panier.
   - *Supprimer des Ouvrages du Panier :* Le client enlève des ouvrages de son panier.

<!--v-->
### Cas d'utilisation du Client :
5. **Passer une Commande :**
   - Le client effectue le processus de passation de commande avec des choix de livraison, de règlement, et de saisie des coordonnées bancaires.

   **Scénarios :**
   - *Choisir les Modalités de Livraison :* Le client sélectionne l'adresse de livraison, le type de livraison, etc.
   - *Choisir le Mode de Règlement :* Le client choisit le mode de règlement pour la commande.
   - *Saisir les Coordonnées Bancaires :* Le client saisit les coordonnées bancaires sur un serveur de paiement sécurisé externe.
   - *Confirmer la Commande :* Le client confirme la commande après une transaction financière réussie.

<!--v-->
### Cas d'utilisation du Client :
6. **Consulter ses Commandes :**
   - Le client peut consulter ses commandes en cours ainsi que l'historique de ses commandes déjà livrées.

   **Scénarios :**
   - *Vérifier les Commandes en Cours :* Le client examine les détails de ses commandes en cours.
   - *Consulter l'Historique des Commandes :* Le client accède à l'historique de ses commandes déjà livrées.

<!--v-->
### Cas d'utilisation du Client :
7. **Créer une Liste de Cadeaux :**
   - Le client peut transformer le contenu de son panier en une liste de cadeaux pour des événements spéciaux.

   **Scénarios :**
   - *Transformer le Panier en Liste de Cadeaux :* Le client convertit le contenu de son panier en une liste de cadeaux.
   - *Saisir les Détails de l'Événement :* Le client spécifie la nature et la date de l'événement ainsi que les prénoms et adresses e-mail des amis concernés.
   - *Générer des Codes Personnalisés :* Un e-mail est généré pour chaque ami avec un code personnalisé pour accéder à la liste.

<!--v-->
### Cas d'utilisation du Client :
8. **Proposer un Avis et un Commentaire :**
   - Le client peut proposer un avis en choisissant parmi un ensemble prédéfini d'appréciations, et peut saisir un commentaire libre de 500 caractères maximum en attente de validation par un Éditeur.

   **Scénarios :**
   - *Donner un Avis :* Le client choisit une appréciation parmi un ensemble prédéfini.
   - *Saisir un Commentaire :* Le client saisit un commentaire libre de 500 caractères maximum.

<!--v-->
### Cas d'utilisation de l'Ami :
- Acteurs Principaux :
   - **Ami (Utilisateur final):** La personne identifiée avec le code reçu par e-mail pour consulter et acheter des cadeaux dans une liste.
- Description :
   1. Consulter une Liste de Cadeaux
   2. Acheter des Cadeaux dans une Liste
- Conditions Spécifiques :
   - L'Ami doit posséder le code d'identification reçu par e-mail pour accéder à la liste de cadeaux.
- Exigences Préalables :
   - Le système doit générer des codes personnalisés et les envoyer par e-mail aux amis identifiés pour accéder à une liste de cadeaux.

Ce cas d'utilisation détaille comment un Ami interagit avec le système pour consulter une liste de cadeaux et acheter des ouvrages dans cette liste. Les scénarios spécifiques fournissent des exemples d'actions que l'Ami peut entreprendre pour accomplir ces tâches.

<!--v-->
### Cas d'utilisation de l'Ami :
1. **Consulter une Liste de Cadeaux :**
   - Après identification de l'ami avec le code reçu par e-mail, la liste des ouvrages sélectionnés non encore choisis est affichée avec leurs caractéristiques, dont le prix.

   **Scénarios :**
   - *Recevoir le Code par E-mail :* L'ami reçoit un e-mail contenant un code personnalisé.
   - *S'Identifier avec le Code :* L'ami accède au site, saisit le code reçu par e-mail pour s'identifier.
   - *Consulter la Liste de Cadeaux :* Une fois identifié, l'ami peut consulter la liste des ouvrages sélectionnés, avec leurs caractéristiques et prix.

<!--v-->
### Cas d'utilisation de l'Ami :
2. **Acheter des Cadeaux dans une Liste :**
   - L'ami désigne un ou plusieurs ouvrages dans la liste des cadeaux restants, saisit ses coordonnées personnelles (celles d'un client), et règle son achat, selon un processus identique au règlement des commandes normales.

   **Scénarios :**
   - *Sélectionner des Ouvrages :* L'ami choisit un ou plusieurs ouvrages dans la liste des cadeaux disponibles.
   - *Saisir les Coordonnées Personnelles :* L'ami saisit ses coordonnées personnelles, qui peuvent être celles d'un client existant ou de nouvelles coordonnées.
   - *Régler l'Achat :* L'ami effectue le règlement de son achat selon le processus standard, en choisissant les modalités de livraison, le mode de paiement, et en saisissant les coordonnées bancaires.


<!--v-->
### Cas d'utilisation de l'Éditeur :
- Acteurs Principaux :
   - **Éditeur (Utilisateur avec des privilèges d'édition):** La personne responsable de l'édition des descriptions d'ouvrages, de la gestion des catégories d'ouvrages, et de l'examen des commentaires.
- Description :
   1. Éditer une Description d'Ouvrage
   2. Gérer les Catégories d'Ouvrages
   3. Examiner les Commentaires en Attente de Validation
- Conditions Spécifiques :
   - L'Éditeur doit être authentifié et avoir des privilèges d'édition pour accéder à ces fonctionnalités.
- Exigences Préalables :
   - L'accès à l'interface d'édition doit être réservé aux utilisateurs ayant des droits d'édition.
   - Le système doit maintenir une liste de catégories d'ouvrages.

Ce cas d'utilisation détaille comment un Éditeur interagit avec le système pour éditer des descriptions d'ouvrages, gérer les catégories d'ouvrages, et examiner les commentaires en attente. Les scénarios spécifiques fournissent des exemples concrets d'actions que l'Éditeur peut entreprendre pour accomplir ces tâches.

<!--v-->
### Cas d'utilisation de l'Éditeur :
1. **Éditer une Description d'Ouvrage :**
   - L'éditeur saisit la description textuelle et le niveau d'expertise (débutant, amateur, chef) de l'ouvrage.

   **Scénarios :**
   - *Sélectionner un Ouvrage à Éditer :* L'éditeur choisit un ouvrage spécifique à éditer.
   - *Saisir la Description Textuelle :* L'éditeur modifie la description textuelle de l'ouvrage.
   - *Spécifier le Niveau d'Expertise :* L'éditeur choisit le niveau d'expertise de l'ouvrage parmi les options (débutant, amateur, chef).
   - *Enregistrer les Modifications :* L'éditeur enregistre les modifications apportées à la description de l'ouvrage.
<!--v-->
### Cas d'utilisation de l'Éditeur :
2. **Gérer les Catégories d'Ouvrages :**
   - L'éditeur peut ajouter, modifier et supprimer des catégories d'ouvrages.

   **Scénarios :**
   - *Ajouter une Nouvelle Catégorie :* L'éditeur crée une nouvelle catégorie pour les ouvrages.
   - *Modifier une Catégorie Existante :* L'éditeur ajuste le nom ou les détails d'une catégorie existante.
   - *Supprimer une Catégorie :* L'éditeur supprime une catégorie qui n'est plus nécessaire.

<!--v-->
### Cas d'utilisation de l'Éditeur :
3. **Examiner les Commentaires en Attente de Validation :**
   - L'éditeur peut afficher la liste des commentaires en attente et les valider ou non par un simple choix.

   **Scénarios :**
   - *Accéder à la Liste des Commentaires en Attente :* L'éditeur visualise la liste des commentaires en attente de validation.
   - *Valider un Commentaire :* L'éditeur approuve un commentaire en le validant pour publication.
   - *Refuser un Commentaire :* L'éditeur rejette un commentaire en le refusant, le retirant de la file d'attente.


<!--v-->
### Cas d'utilisation du Gestionnaire :
#### Acteurs Principaux :
- **Gestionnaire (Utilisateur avec des privilèges de gestion):** La personne responsable de la gestion du catalogue, du stock et du suivi des ventes.

#### Description :

1. **Gérer le Catalogue :**
   - Le gestionnaire peut ajouter un ouvrage avec ses données factuelles (éditeur, nombre de pages, date de parution, etc.), modifier un ouvrage, supprimer un ouvrage, et afficher le catalogue.

   **Scénarios :**
   - *Ajouter un Nouvel Ouvrage au Catalogue :* Le gestionnaire ajoute un nouvel ouvrage en fournissant ses données factuelles telles que l'éditeur, le nombre de pages, la date de parution, etc.
   - *Modifier un Ouvrage Existants :* Le gestionnaire ajuste les détails d'un ouvrage existant, comme sa date de parution ou le nombre de pages.
   - *Supprimer un Ouvrage du Catalogue :* Le gestionnaire retire un ouvrage du catalogue qui n'est plus disponible.
   - *Afficher le Catalogue :* Le gestionnaire peut visualiser l'ensemble du catalogue d'ouvrages.

2. **Gérer le Stock :**
   - Le gestionnaire peut enregistrer une entrée en stock, enregistrer une sortie exceptionnelle du stock, afficher le stock, et rechercher selon le niveau de stock.

   **Scénarios :**
   - *Enregistrer une Entrée en Stock :* Le gestionnaire enregistre l'arrivée de nouvelles unités d'un ouvrage dans le stock.
   - *Enregistrer une Sortie Exceptionnelle du Stock :* Le gestionnaire déclare une sortie exceptionnelle du stock, par exemple en cas de dommages.
   - *Afficher le Stock :* Le gestionnaire peut voir l'état actuel du stock d'ouvrages.
   - *Rechercher selon le Niveau de Stock :* Le gestionnaire peut rechercher les ouvrages en fonction de leur niveau de stock.

3. **Suivre les Ventes :**
   - Le gestionnaire peut déterminer les ventes selon différents critères (période, niveau de détail, etc.).

   **Scénarios :**
   - *Déterminer les Ventes sur une Période :* Le gestionnaire obtient des informations sur les ventes pendant une période spécifique.
   - *Obtenir des Détails sur les Ventes :* Le gestionnaire peut accéder à des détails plus précis sur les ventes, comme le nombre d'unités vendues par ouvrage.

#### Conditions Spécifiques :
- Le Gestionnaire doit être authentifié et avoir des privilèges de gestion pour accéder à ces fonctionnalités.

#### Exigences Préalables :
- L'accès à l'interface de gestion doit être réservé aux utilisateurs ayant des droits de gestion.
- Le système doit maintenir une base de données à jour du catalogue d'ouvrages, du stock, et des informations de vente.

Ce cas d'utilisation détaille comment un Gestionnaire interagit avec le système pour gérer le catalogue, le stock, et suivre les ventes. Les scénarios spécifiques fournissent des exemples d'actions que le Gestionnaire peut entreprendre pour accomplir ces tâches.

<!--v-->
### Cas d'utilisation de l'Administrateur :

#### Acteurs Principaux :
- **Administrateur (Admin):** L'administrateur du système.

#### Description :

1. **Gérer les Utilisateurs du Back Office :**
   - L'administrateur a la capacité de gérer les utilisateurs du back office, y compris les éditeurs, les gestionnaires et d'autres administrateurs.
   - Il peut ajouter de nouveaux utilisateurs, modifier les informations existantes, ou supprimer des comptes d'utilisateurs du back office.
   
   **Scénarios :**
   - *Ajouter un Nouvel Utilisateur :* L'administrateur ajoute un nouvel éditeur en spécifiant son nom, son adresse e-mail, et son rôle dans le back office.
   - *Modifier les Informations d'un Utilisateur Existants :* L'administrateur modifie les informations d'un gestionnaire en mettant à jour son adresse e-mail et en ajustant ses droits d'accès.
   - *Supprimer un Compte d'Utilisateur :* L'administrateur supprime le compte d'un administrateur qui ne fait plus partie de l'équipe.

2. **Gérer les Clients :**
   - L'administrateur peut gérer les clients du système, ce qui inclut l'ajout de nouveaux clients, la modification des informations existantes, et la suppression de comptes clients si nécessaire.
   
   **Scénarios :**
   - *Ajouter un Nouveau Client :* L'administrateur ajoute un nouveau client en fournissant les détails requis tels que le nom, l'adresse, l'e-mail, etc.
   - *Modifier les Informations d'un Client Existants :* L'administrateur ajuste les informations d'un client en mettant à jour son adresse ou d'autres détails.
   - *Supprimer un Compte Client :* L'administrateur supprime le compte d'un client sur demande de ce dernier ou en cas de violation des conditions d'utilisation.

3. **Maintenir le Site :**
   - L'administrateur peut prendre des mesures pour maintenir le bon fonctionnement du site, ce qui peut inclure des actions telles que l'application de mises à jour logicielles, la gestion des ressources du serveur, et la surveillance des performances.

   **Scénarios :**
   - *Appliquer des Mises à Jour Logicielles :* L'administrateur planifie et applique les mises à jour logicielles nécessaires pour garantir la sécurité et la stabilité du site.
   - *Gérer les Ressources du Serveur :* L'administrateur surveille et ajuste les ressources du serveur en fonction des besoins du site pour assurer une performance optimale.
   - *Surveiller les Performances :* L'administrateur utilise des outils de surveillance pour identifier les problèmes potentiels et prend des mesures pour les résoudre.

#### Conditions Spécifiques :
- L'administrateur doit être authentifié pour accéder aux fonctionnalités de gestion du back office et du site.

#### Exigences Préalables :
- Accès aux outils d'administration du site.
- Connaissance des politiques de gestion des utilisateurs et des clients.

Ce cas d'utilisation détaille comment l'Administrateur peut maintenir le site en gérant les utilisateurs du back office, en gérant les clients, et en prenant des mesures pour assurer le bon fonctionnement général du site. Les scénarios spécifiques fournissent des exemples concrets d'actions que l'administrateur peut entreprendre dans ces domaines.

<!--v-->
##### Cas d'utilisation

<!--v-->
##### Cas d'utilisation de l'Internaute
1) Cas d'utilisation de l'Internaute
- Rechercher des ouvrages : l'application offre aux internautes plusieurs méthodes de recherche.
- Une recherche textuelle dans les descriptions.
- Une recherche avancée par catégories : niveau d'expertise, catégorie d'ouvrage, tranche de prix.
- Une recherche par les caractéristiques de l'ouvrage : titre, auteur, numéro ISBN.
- Une recherche selon la popularité : avis des clients et ventes réalisées.

Seuls les ouvrages disponibles en stock doivent apparaître dans les listes de résultat.

- Consulter un ouvrage : l'ouvrage trouvé par l'internaute est présenté en détail avec la photo de sa couverture, ses caractéristiques, sa description, l'avis des clients, un accès aux commentaires.


<!--v-->
##### Cas d'utilisation du Client
2) Cas d'utilisation du Client
- S'enregistrer : le futur client doit fournir des informations obligatoires (nom, prénom, adresse, mail, login, mot de passe) et peut fournir des informations facultatives supplémentaires (âge, téléphone, etc.).
- Se connecter : le client enregistré se connecte par saisie de son login et de son mot de passe.
- Rechercher des ouvrages et Consulter un ouvrage (cf. ci-dessus).
- Sélectionner des ouvrages dans son panier : le client peut en ajouter, simplement en les désignant, en supprimer, en changer la quantité. Il est informé à chaque instant du nombre d'articles et du montant courant du panier.
- Passer une commande : ce processus de passation de commande par le client comporte le choix des modalités de livraison (adresse de livraison, type de livraison), le choix du mode de règlement, la saisie des coordonnées bancaires sur un serveur de paiement sécurisé externe et la confirmation d'achat en cas de succès de la transaction financière.
- Consulter ses commandes : le client peut consulter ses commandes en cours et l'historique de ses commandes déjà livrées.
- Créer une liste de cadeaux :leclientpeuttransformerlecontenudesonpanier en une liste de cadeaux. Il doit ensuite saisir la nature et de la date de l'événement fêté, les prénoms et adresses mail des amis concernés par la liste. Un mail est généré pour chaque ami avec un code personnalisé lui permettant ultérieurement l'accès à la liste.
- Proposer un avis : le client effectue un simple choix parmi un ensemble prédéfini d'appréciations.
- Proposer un commentaire : le client saisit un texte libre de 500 caractères au maximum qui est enregistré en attente de validation par un Éditeur.

<!--v-->
##### Cas d'utilisation de l'Ami
3) Cas d'utilisation de l'Ami
- Consulter une liste de cadeaux : après identification de l'ami avec le code reçu par mail, la liste des ouvrages sélectionnés non encore choisis est affichéeavec leurs caractéristiques, dont le prix.
- Acheter des cadeaux dans une liste : l'ami désigne un ou plusieurs ouvrages dans la liste des cadeaux restants, saisit ses coordonnées personnelles (celles d'un client) et règle son achat, selon un processus identique au règlement des commandes normales.

<!--v-->
##### Cas d'utilisation de l'Éditeur
4) Cas d'utilisation de l'Éditeur
- Éditer une description d'ouvrage : l'éditeur saisit la description textuelle et le niveau d'expertise (débutant, amateur, chef) de l'ouvrage.
- Gérer les catégories d'ouvrages : l'éditeur peut ajouter, modifier et supprimer des catégories.
- Examiner les commentaires en attente de validation : l'éditeur peut afficherla liste des commentaires en attente et les valider ou non par un simple choix.

<!--v-->
##### Cas d'utilisation du Gestionnaire (à détailler ultérieurement)
5) Cas d'utilisation du Gestionnaire (à détailler ultérieurement)
- Gérer le catalogue : le gestionnaire peut ajouter un ouvrage avec ses données factuelles (éditeur, nombre de pages, date de parution, etc.), modifier un ouvrage, supprimer un ouvrage et afficherle catalogue.
- Gérer le stock : le gestionnaire peut enregistrer une entrée en stock, enregistrer une sortie exceptionnelle du stock, afficherle stock, rechercher selon le niveau de stock.
- Suivre les ventes : le gestionnaire peut déterminer les ventes selon différents critères (période, niveau de détail, etc.).

<!--v-->
##### Cas d'utilisation de l'Administrateur (à détailler ultérieurement)
6) Cas d'utilisation de l'Administrateur (à détailler ultérieurement)
- Maintenir le site : l'administrateur peut gérer les utilisateurs du back office (éditeurs, gestionnaires, administrateurs), gérer les clients, etc.

<!--v-->
3. **LES EXIGENCES NON FONCTIONNELLES**

Elles sont classées en trois catégories : facilité d'utilisation, efficacitéet sécurité.

1. **Facilité d'utilisation**
- Présentation des pages du site simple et agréable à l'œil.
- Seules les fonctionnalités utilisables selon le rôle joué (internaute, client enregistré, ami, etc.) doivent apparaître.
- Aide en ligne systématique et uniforme sur tout le site.
- Formulaire de contact disponible et réactivité des réponses.
2. **Efficacité**
- Pas de durée de recherche supérieure à 5 secondes avant l'affichagedes premiers résultats.
- Pic de charge absorbable jusqu'à 100 connexions simultanées.
3. **Sécurité**
- Paiement sécurisé.
- Pas de conservation des coordonnées bancaires après achat.
- Durée de vie du panier limitée à la session.

<!--l-->
4. **UNE ÉBAUCHE D'ARCHITECTURE FONCTIONNELLE**

Le front office et le back office sont séparés. Cela correspond à une première ébauche d'architecture fonctionnelle en deux paquets.