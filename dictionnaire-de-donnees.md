# Dictionnaire de données
Plusieurs quizz, chaque quizz a plusieurs questions à l'intérieur. Il y a 4 réponses possibles pour chaque question. 

Un quizz comporte : Un titre, un auteur, un ou plusieurs thèmes, un ou plusieurs sujets, une ou plusieurs questions, plusieurs réponses, un niveau, et une ou plusieurs informations


## Quizz (`quizz`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| title | VARCHAR(255) | NOT NULL | Le nom |
| question_id | ENTITY | NULL | Le(s) question(s) attaché(s) au quizz |
| author_id | ENTITY | NULL | L'auteur attaché au quizz |
| level_id | ENTITY | NULL | Le niveau attaché au quizz |
| information_id | ENTITY | NULL | Le(s) informations(s) attaché(s) au quizz |
| subject_id | ENTITY | NULL | Le(s) sujet(s) attaché(s) au quizz |
| theme_id | ENTITY | NULL | Le(s) theme(s) attaché(s) au quizz |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Auteur (`author`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| name | VARCHAR(255) | NOT NULL | Le nom |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Thème (`theme`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| title | VARCHAR(255) | NOT NULL | Le nom |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Sujet (`subject`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| title | VARCHAR(255) | NOT NULL | Le nom |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Question (`question`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| question | VARCHAR(255) | NOT NULL | La question |
| response_id | ENTITY | NULL | Les réponses attachés à cette question |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Réponse (`response`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| response_1 | VARCHAR(255) | NOT NULL | La response 1 |
| response_2 | VARCHAR(255) | NOT NULL | La response 2 |
| response_3 | VARCHAR(255) | NOT NULL | La response 3 |
| response_4 | VARCHAR(255) | NOT NULL | La question 4 |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Niveau (`level`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| title | VARCHAR(255) | NOT NULL | Le nom |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La date de dernière modification |


## Information (`information`)
| Champ | Type | Spécificités | Description |
| - | - | - | - |
| id | INT | PRIMARY KEY, UNSIGNED, NOT NULL, AUTO_INCREMENT | L'identifiant de notre liste |
| title | VARCHAR(255) | NOT NULL | Le nom |
| description | TEXT | NOT NULL | Le texte d'information |
| created_at | TIMESTAMP | NOT NULL, DEFAULT CURRENT_TIMESTAMP | La date de création |
| updated_at | TIMESTAMP | NULL | La description |