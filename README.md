Le but de ce TP est de mettre en pratique les différentes connaissances acquises durant les séances de TD et TP.
Le lien du github est : git@github.com:Aiduknow/jazz-poo.git

Réponses aux différenets questions : 

ETAPE 5:
1) Spring Web : est une partie du framework Spring qui permet de créer des applications web basées sur Java.
   Il fournit des outils pour gérer les requêtes HTTP, les routes, les contrôleurs, les modèles de vue et les formulaires.
   Il facilite également l'intégration avec d'autres technologies comme les bases de données et les services web.
   En résumé, Spring Web est une plate-forme complète pour la création d'applications web en utilisant Java.

2) JPA : JPA est une spécification Java pour la gestion de la persistance des données qui permet de stocker et
   récupérer des objets Java à partir d'une base de données en utilisant des annotations ou des fichiers XML pour
   définir les relations entre les objets. Il génère automatiquement les requêtes SQL nécessaires et est
   supporté par plusieurs implémentations populaires.  Il est utilisé pour simplifier la gestion des données dans les applications Java.

3) Hibernate : Hibernate est un framework open-source pour la gestion de la persistance des données en Java.
   Il est une implémentation de JPA (Java Persistence API) qui permet de stocker et récupérer des objets Java
   à partir d'une base de données en utilisant des annotations ou des fichiers XML pour définir les relations entre les objets.


4) H2 : H2 est un moteur de base de données relationnelle écrit en Java. Il est open-source, léger et embarquable,
   ce qui signifie qu'il peut être intégré directement dans une application Java sans nécessiter l'installation
   d'un serveur de base de données séparé. Il prend en charge les normes SQL standard et est compatible
   avec les principaux systèmes de gestion de bases de données tels que MySQL, PostgreSQL et Oracle.


5) Devtools :  est un ensemble d'outils pour les développeurs qui facilite le développement et le débogage d'applications web.
   Il peut inclure des fonctionnalités telles que la surveillance en temps réel des modifications de code, la rechargement automatique
   des modifications, l'inspection des éléments HTML et CSS, l'analyse des performances et des erreurs, et la console de débogage.


6) ThymeLeaf : Thymeleaf est un template engine (moteur de rendu de document) écrit en Java.
Principalement conçu pour produire des vues Web il fournit un support pour la génération de documents HTML,
XHTML, JavaScript et CSS. 


ETAPE 12 : 
1) Avec quelle partie du code avons-nous paramétré l'url d'appel/greeting ?
Nous l'avons paramétré à l'aide de HelloWorldController  : @GetMapping("/greeting")

2)  Nous choisissons le fichier HTML à l'aide de :
return "greeting"

3) Nous envoyons le nom de l'utilisateur à l'aide de :
$nomTemplate dans : <p th:text="'Bonjour ' + ${nomTemplate} + ' !'" />


ETAPE 17 : 
Nous pouvons remarquer qu'il y a apparition d'une nouvelle table Address

ETAPE 18 :
Hibernate est un outil ORM qui nous permet d'interagir avec une base de données en utilisant des objets Java.
Hibernate est utilisée pour générer une table. En effet, les champs sont annotés par : 
@Id pour la clé primaire,@Column pour les colonnes, et @ManyToOne pour les relations. 

ETAPE 20:
Select * from address;
ID  	CONTENT  	CREATION  
(no rows, 3 ms)
Non nous ne voyons pas tout le contenu de data.sql (voir ci-dessus)


ETAPE 22 : 

L’annotation @Autowired permet d’activer l’injection automatique de dépendance. 
Elle peut être placée sur un constructeur, une méthode ou directement sur un attribut. 
Le Spring Framework va chercher le bean du contexte d’application dont le type 
est applicable à chaque paramètre du constructeur, aux paramètres de la méthode ou à l’attribut. 

ETAPE 26 :
select * from address;
ID  	CONTENT  	CREATION  	NOM  

ETAPE 30 :

