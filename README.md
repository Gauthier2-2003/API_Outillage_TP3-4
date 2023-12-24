Dependencies:
-------------------------
Spring Web : La dépendance spring-web contient des utilitaires communs spécifiques au Web pour les environnements Servlet et Portlet, tandis que spring-webmvc permet le support MVC pour les environnements Servlet. Comme spring-webmvc a spring-web comme dépendance, il n'est pas nécessaire de définir explicitement spring-web lorsque vous utilisez spring-webmvc.

JPA : JPA a pour objectif d'unifier et de faciliter l'accès aux différents types de magasins de persistance, qu'il s'agisse de systèmes de bases de données relationnelles ou de magasins de données NoSQL.

Hibernate : Hibernate est utilisé pour accéder à la couche de données. Il s'agit d'un framework de persistance qui facilite la gestion des données dans une application Java.

H2 : H2 est une base de données embarquée, open-source et en mémoire. Il s'agit d'un système de gestion de base de données relationnelle écrit en Java. Il stocke les données en mémoire et ne les fait pas persister sur le disque.

DevTools : Les DevTools de Spring Boot permettent de récupérer les changements et de redémarrer l'application automatiquement lors de la modification du code source.

Thymeleaf : Thymeleaf est un moteur de modèles Java côté serveur pour les environnements Web et autonomes. Il est capable de traiter du HTML, du XML, du JavaScript, du CSS et même du texte brut.

Question 13:
-------------------------

1/  Avec quelle partie du code avons-nous param�tr� l'url d'appel /greeting ?
	Nous avons paramétré l'URL d'appel /greeting dans la méthode HelloWorldController après avoir utilisé l'annotation @GetMapping, qui est utilisée pour mapper les requêtes HTTP GET sur des méthodes de traitement spécifiques. Dans notre cas, cette méthode prend comme paramètre l'URL /greeting.

2/  Avec quelle partie du code avons-nous choisi le fichier HTML à afficher ?
	Nous avons choisi le fichier HTML à afficher dans la méthode appelée après avoir reçu une requête vers /greeting. Cette méthode s'appelle greeting et prend un paramètre name, qui n'est pas requis et a une valeur par défaut si l'utilisateur ne fournit pas de paramètre. Cette méthode retourne un fichier HTML appelé greeting.

3/  Comment envoyons-nous le nom � qui nous disons bonjour avec le second lien ?
	Pour envoyer le nom auquel nous disons bonjour avec le deuxième lien (http://localhost:8080/greeting?name=ENSIM), nous utilisons le paramètre name dans l'URL, qui est géré par @RequestParam. L'annotation @RequestParam permet à Spring d'extraire des données d'entrée transmises sous forme de requête, de données de formulaire ou d'autres données personnalisées arbitraires.

Question 17:
--------------------
Oui, la classe Adresse est ajoutée. Après avoir défini une entité Adresse, Hibernate peut générer la classe correspondante.

Question 20:
--------------------
Oui, je le vois. Voici les données affichées :

22 rue alvebrt eben - 2023-12-18 18:26:51.516783
16 bd charles nicolle, 72000 le Mans - 2023-12-18 18:26:51.51778

