# TD_TODO_LIST FLASK
TD TODO LIST FLASK

REPONSE DES QUESTIONS

exercice 1**********

1. role de l'objet app permet de représente l’application web.et definir les routes ainsi gerer les requetes http
2. lorque on ouvrire http://127.0.0.1:5000/ le serveur Flask démarre, et cherche la route correspondante, pour exécute la fonction associée, puis retourne le résultat.

exercice 2*******

1 . Lorsque l’on accède à l’URL /, Flask reçoit la requête et exécute la fonction définie avec @app.route("/").
Cette fonction utilise render_template() pour chercher le fichier home.html dans le dossier templates, et générer le contenu HTML, et l'affiche sur l'ecran 
2. Flask ne trouvera pas le fichier et affichera une erreur car le fichier est renomée

exercice 3********

1. {% if task.done %} vérifie si task est faite (True).
Si elle est faite le texte est barré avec <s> ou saffiche faite avec color red.
Sinon affichage normal
2. Python prépare les données, par centre le template ninja2 s'affiche les donnes.
   
exercice 4*******

1. pour facilite la maintenance (bug) et eviter la répétition de code ainsi facile a modifier
   
exercice 5*********

role db : c'est l'instance de la connexion à la base de données définie dans SQLALCHEMY_DATABASE_URI

exercice 6********

1. le fichier de base de données sur Flask-SQLALCHEMY
2. db.create_all() Crée la base et les tables si elles n'existent pas
   
exercice 7**********

1 role db.session.ad() : C’est comme mettre une modification “en attente
role db.session.commit() : c'est la confirmation finle 

question synthese:********************

1 .
L’utilisateur accède à la page d’accueil
Le formulaire envoie une requête POST vers /add
La fonction retourne redirect("/")

2 .
on manipule des objets Python au lieu d’écrire des requêtes SQL
réduit les risques d’injection SQL
fonctionne avec différentes bases

3. bonnes pratiques pour les templates Jinja2
Utilise l’héritage de templates.
Utilise des blocs {% block %} pour garder un code lisible.
