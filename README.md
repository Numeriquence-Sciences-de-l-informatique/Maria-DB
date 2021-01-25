# Maria-DB

I. Le modèle relationnel 
Consiste à représenter les donnés dans des tables

définitions :
- Dans une table, chaque ligne constitue un enregistrement
- Las attributs d'une sont les noms de ses colonnes
- Le degré, ou arité d'une table est le nombre de ses colonnes
- La cardinalité d'une table est le nombre de ses enregistrements
- le domaine d'un attribut est son type : int, float, string, boolean !
- **La Clef Primaire** d'une table est l'attribut permettant d'identifier de manière unique un enregistrement d'une table
- **Une Clef étrangère** est un attribut d'une table faisant référence à la clé primaire d'une table


II. Le langage SQL
> Les mots-clés SQL en majuscule et avec un `;`à la fin de chaque **requête**
> Pour nommer des champs lors d'une jointure, on peut écrire le nom de la table puis le caractère `.` et sa var => `SHOW TABLES Jeu.IdGame from Jeu`

> CREATE DATABASE <NameOfDB>;
  Permet de créer une base de données sur un serveur
> SHOW DATABASES;
  Permet de visualiser l'ensembles des DB présente sur le serveur de l'utilisateur.
> USE <NameOfDB>
  Permet d'utiliser la DB en question
> CREATE TABLE <NameTable>(Attribut1 TypeAttribut1 ContrainteAttribut1, Attribut2 TypeAttribut2 ContrainteAttribut2, ...);
  Permet de créer une table avec différentes types de donnés (exemple de types de donnés utilisés) :
  - VARCHAR(x) : chaîne de caractère avec une taille maximale de x caractères
  - INT : entier de 32 bits
  - NULL : Valeur NULL comme None en Python
  - DATE : (année/mois/jours)
> INSERT INTO <NameTable>(liste Attributs) VALUES (valeur 1, ... valeur x);
  Permet d'insérer un enregistrement dans une table en précisant les attributs
> DROP TABLE <NameTable>;
  Permet de supprimer une table présente dans une DB
> SHOW TABLES;
  Permet de visionner toutes les tables présentes dans une DB
> SHOW CREATE TABLES <NameTable>;
  Permet de visualiser la structure d'une table présente dans une DB
> UPDATE <NameTable> SET Attribut=valeur WHERE condition;
  Permet de mettre à jour un ou plusieurs enregistrements d'une table
> SELECT * FROM <NameTable>;
  Permet de visualiser les enregistrements, attributs et valeurs d'une table présente dans DB.
