# mld-mcd-sql

Cet exercice a été réalisé dans le cadre d’une évaluation lors de ma formation à l’école O’clock.
Avant de réaliser les wireframes, il nous était demandé de créer la structure de la base de données de ce site de quizz.
J’ai commencé par réaliser le MCD : Modèle conceptuel des données, afin de comprendre facilement comment les différents éléments sont liés entre eux.

Par la suite, j’ai rédigé le dictionnaire de données, afin d’avoir une idée plus précise du type de données attendus dans la base de données. Par exemple si une donnée peut être null ou non, de quel type de données la base de données attends, etc. (integer, timestamp, varchar, etc.)
Après, j’ai créé le MLD (modèle logique de données) via MySQL Workbench afin de définir toutes les relations pour qu’elles soient ensuite compréhensible par notre logiciel de gestion de base de données, dans notre cas phpMyAdmin : 


Enfin, j’ai exporté dans un fichier .sql la base de donnée (généré par MySQL Workbench) afin de l’importer sur phpMyAdmin pour avoir une base de données fonctionnelle.
