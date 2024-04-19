Présentation de la startup : BoxeGear

Domaine d'activité :
BoxeGear se positionne dans le secteur de l'équipement de boxe, offrant une gamme complète de produits de haute qualité pour les pratiquants de boxe de tous niveaux, 
des débutants passionnés aux professionnels de haut niveau.

Vision / Stratégie :
Notre vision est de devenir le leader mondial de l'équipement de boxe en offrant des produits innovants, de haute qualité et personnalisés, tout en favorisant une culture de l'excellence et 
de l'engagement envers nos clients. Nous nous efforçons de créer une communauté passionnée de boxeurs et de passionnés de sports de combat, tout en repoussant les limites de l'innovation dans notre domaine.

Diagramme "Bête à cornes" :

![image](https://github.com/markosm77/analyse_besoin_boxe/assets/96230455/54897e6c-40f6-4af4-8e66-66545705805c)


Le diagramme "Bête à cornes" met en évidence les éléments clés de BoxeGear, notamment notre offre de produits, notre engagement envers la qualité et l'innovation, 
notre relation avec les clients et notre positionnement sur le marché de l'équipement de boxe.


Diagramme de pieuvre :

![image](https://github.com/markosm77/analyse_besoin_boxe/assets/96230455/6bf3394a-e572-4400-85d8-b3c15b922306)

Le diagramme de pieuvre illustre les différentes parties prenantes de BoxeGear, y compris nos fournisseurs, nos distributeurs, nos clients, notre équipe interne et d'autres acteurs du marché,
ainsi que les interactions entre eux.

La problématique :
Dans le cadre de notre activité, nous avons identifié un problème majeur lié à l'ajustement et à la qualité des gants de boxe pour les pratiquants. 
De nombreux boxeurs rencontrent des difficultés pour trouver des gants qui leur vont parfaitement et qui offrent un confort optimal tout en garantissant une protection adéquate. 
Cela peut entraîner des blessures et une expérience de pratique moins satisfaisante.
Nous cherchons à résoudre ce problème en développant des solutions innovantes pour la conception et la personnalisation des gants de boxe.

Exigences Techniques:
BoxeGear envisage de mettre en place une solution innovante pour améliorer l’expérience de ses clients. Cette solution comprend un site web et une application mobile, tous deux construits avec React, qui permettent aux utilisateurs de prendre une photo de leur main. Cette photo est ensuite analysée par des modèles d’IA pour recommander des gants de boxe personnalisés.
L’architecture de la solution est organisée en couches :
Couche de présentation : Construite avec React pour le site web et React Native pour l’application mobile, cette couche permet aux utilisateurs de naviguer à travers les produits, de prendre des photos de leur main, et de recevoir des recommandations personnalisées.
Couche application : Cette couche contient la logique métier et les modèles d’IA. Elle utilise FastAPI pour la gestion des API Restful, Alembic pour la gestion des migrations de la base de données, et SQLAlchemy comme ORM. Les modèles d’IA intégrés sont :
DLRM (Deep Learning Recommendation Model) pour recommander des produits en fonction des préférences et du style de boxe de l’utilisateur.
Gorse pour recommander des articles à partir de sources multiples.
MediaPipe Hand Landmarker et BlazeHand pour détecter les points clés de la main à partir des photos prises par les utilisateurs.
Couche données : Cette couche gère le stockage des données des utilisateurs, des produits, des préférences des utilisateurs, des photos des mains des utilisateurs, etc. Elle utilise une base de données classique.
En ce qui concerne l’infrastructure, la solution sera hébergée sur le cloud, ce qui permet une grande flexibilité, une évolutivité facile et une haute disponibilité. Le déploiement continu (CD) et l’intégration continue (CI) seront mis en place pour assurer un développement et une livraison de logiciels rapides et fiables. Cela permettra des mises à jour régulières et garantira que le logiciel fonctionne correctement à chaque nouvelle version.
En combinant ces technologies, BoxeGear peut offrir une expérience utilisateur personnalisée et innovante, aidant les boxeurs à trouver les gants parfaits pour leurs besoins spécifiques. Cette solution permettra à BoxeGear de se rapprocher de sa vision de devenir le leader mondial de l’équipement de boxe.
Nous utiliserons également Snowflake avec du Spark pour le stockage et le traitement de données avant de les intégrer dans nos modèles d'IA.

Modèles d'IA : 
DLRM (Deep Learning Recommendation Model)123 : DLRM est un modèle de recommandation basé sur l’apprentissage profond. Il combine les principes du filtrage collaboratif et des approches basées sur l’analyse prédictive, ce qui lui permet de travailler efficacement avec des données à l’échelle de la production et de fournir des résultats de pointe1. Dans le modèle DLRM, les caractéristiques catégorielles sont traitées à l’aide d’incorporations, tandis que les caractéristiques continues sont traitées avec un perceptron multicouche (MLP). Ensuite, les interactions de second ordre de différentes caractéristiques sont calculées explicitement1.
Gorse456 : Gorse est un système de recommandation open-source écrit en Go. Il vise à être un système de recommandation open-source universel qui peut être facilement introduit dans une grande variété de services en ligne4. En important des articles, des utilisateurs et des données d’interaction dans Gorse, le système formera automatiquement des modèles pour générer des recommandations pour chaque utilisateur4.
MediaPipe Hand Landmarker789 : MediaPipe Hand Landmarker est une tâche qui vous permet de détecter les points clés des mains dans une image7. Vous pouvez utiliser cette tâche pour localiser les points clés des mains et rendre des effets visuels sur eux7. Cette tâche fonctionne sur des données d’image avec un modèle d’apprentissage automatique comme données statiques ou un flux continu et produit des points clés de main en coordonnées d’image, des points clés de main en coordonnées mondiales et la latéralité (main gauche/droite) de plusieurs mains détectées7.
BlazeHand101112 : BlazeHand est un modèle d’apprentissage automatique qui détecte les points clés de la main10. Comme il peut détecter des mouvements de main détaillés, il peut être appliqué à la reconnaissance des gestes10. BlazeHand se compose de deux modèles, BlazePalm et BlazeHand. Après avoir détecté la position de la main à partir de l’image d’entrée avec BlazePalm, les points clés de la main sont détectés à partir de l’image de la main avec BlazeHand10.

Politique de confidentialité de BoxeGear :
Chez BoxeGear, nous attachons une grande importance à la protection de la vie privée et à la sécurité des données de nos clients. 
Notre politique de confidentialité vise à garantir que toutes les informations personnelles collectées sont traitées de manière sécurisée et conforme aux lois et
réglementations en vigueur. Nous collectons uniquement les données nécessaires pour fournir nos services et améliorer l'expérience utilisateur, et nous nous
engageons à ne pas partager ces informations avec des tiers sans consentement préalable. Notre politique de confidentialité détaille les types de données que 
nous collectons, la manière dont nous les utilisons et les mesures que nous prenons pour garantir leur sécurité.

Conditions Générales d'Utilisation (CGU) :

Les Conditions Générales d'Utilisation (CGU) de BoxeGear établissent les règles et les conditions d'utilisation de notre site web, 
de nos applications mobiles et de nos services. En accédant à nos plateformes et en utilisant nos services, les utilisateurs acceptent de se conformer à ces conditions. 
Les CGU couvrent des aspects tels que les droits et responsabilités des utilisateurs et de BoxeGear, les restrictions d'utilisation, 
la propriété intellectuelle, la confidentialité des données, les règles de conduite et les dispositions juridiques applicables.

Conditions Générales de Vente (CGV) :

Les Conditions Générales de Vente (CGV) de BoxeGear définissent les termes et les conditions régissant les achats de produits et services sur notre plateforme.
Elles couvrent des éléments tels que la description des produits, les prix et les modalités de paiement, les frais de livraison, 
les conditions de retour et de remboursement, les garanties, les limitations de responsabilité et les dispositions juridiques applicables. 
En effectuant un achat sur BoxeGear, les clients acceptent automatiquement nos CGV.

En intégrant ces éléments dans notre stratégie globale, nous nous engageons à assurer la transparence, la confiance et la satisfaction de nos clients
tout en respectant les normes les plus élevées en matière de protection des données et de réglementation commerciale.
