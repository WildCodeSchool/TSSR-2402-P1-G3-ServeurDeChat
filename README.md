# **Implémentation d'un serveur de messagerie instantanée (chat)**

![RocketChat](attachments/rocketchat_original.png)

Ce document est réservé à usage interne, il ne peut en aucun cas être divulgué à des tiers.

Dernière mise à jour du Document : **22 mars 2024**

## **Sommaire**

1. Présentation du projet et objectifs finaux

2. Introduction : mise en contexte

3. Présentation des membres du groupe et de leur rôles

4. Choix techniques et contraintes

5. Difficultés rencontrées

6. Solutions et/ou Alternatives trouvées pour palier aux problèmes

7. Next-Step : Améliorations possibles envisagées

### **1. Présentation du Projet et Objectifs finaux**

Le projet consiste à installer le software **_Rocket.Chat_** sur notre Serveur Debian, afin que celui-ci donne accés à toutes les fonctionnalités qu'offre le logiciel sur nos 2 ordinateurs Clients (Ubuntu et Windows).

La Deadline du projet est fixée au **vendredi 22 mars 2024**.

Une présentation de l'avancement du projet sera effectué le vendredi 22 mars 2024.

L'équipe est fière d'avoir relever ce défi, nous avons atteint l'objectif principal qui était de mettre en place un service de messagerie, basé sur **_Rocket.Chat_**.

Nous avons par la même occasion atteint l'objectif secondaire, qui était la personnalisation des emojis et des réactions, vous pouvez retrouver la méthode pour les modifier dans le fichier USER_GUIDE.md
Cette partie sera abordé lors de la démonstration

La documentation jointe au projet est constitué de 3 fichiers au format markdown :

- une documentation générale (README.md)
- une documentation administrateur (INSTALL.md)
- une documentation utilisateur (USER_GUIDE.md)

Un dépôt GitHub a été créé à cet effet : [TSSR-2402-P1-G3-ServeurDeChat](https://github.com/WildCodeSchool/TSSR-2402-P1-G3-ServeurDeChat)

### **2. Introduction : Mise en contexte**

Le projet devrait faciliter grandement la communication entre nos collaborateurs, et permettra ainsi d'avancer avec plus d'efficacité sur les projets en cours.

### **3. Présentation des membres du groupe et de leur rôles**

Le Projet **_Rocket.Chat_** est composé des membres de la DSI :

* **Anaïs Lenglet**
* **Pierre Girard**
* **Julien Guillot**
* **Yanis Hortholary**
* **Anthony Javault**

Rappel des rôles et responsabilités :

- Rôle du _Scrum Master_ (SM) :
    >
    > Le SM est le garant de la bonne application de la méthode Scrum. Il est responsable de la communication entre les membres de l'équipe et de la bonne réalisation des tâches.
    >        
- Rôle du _Product Owner_ (PO) :
    >
    > Le PO est le représentant du client. Il est responsable de la définition des besoins et de la priorisation des tâches. Il est le garant de la qualité du produit final.
    >

Sont nommés pour la première semaine de Projet (Sprint 1) :

* PO : **Julien Guillot**
* SM : **Yanis Hortholary**
            
Sont nommés pour la seconde semaine de Projet (Sprint 2) :

* PO : **Anaïs Lenglet**
* SM : **Anthony Javault**

Attribution des tâches/activités par membre :

|Activités|**Anaïs Lenglet**|**Pierre Girard**|**Julien Guillot**|**Yanis Hortholary**|**Anthony Javault**|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Configuration du Serveur||x|x|||
|Configuration des Clients||x|x|x||
|Tests Serveur||x|x|x|x|
|Tests Clients|x|x|x|x|x|
|Documentation|x||||x|
|Revue Documentation|x||x|x||
|Préparation Présentation|x|x||x|x|

### **4. Choix techniques et contraintes**

En ce qui concerne la version serveur, **_Rocket.Chat_** étant plus optimisé pour Debian, le choix est évident.

Le Serveur est par conséquent sous Linux Debian 12.5 :

- Nom : SRVLX01
- Compte : root
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.10/24

Les clients sont respectivement sous OS Windows 10 (client 1) Ubuntu 22.04 LTS (client 2).

Pour le client Microsoft Windows 10 Pro 22H2 : 

- Nom : CLIWIN01
- Compte utilisateur : wilder (dans le groupe des admins locaux)
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.20/24

Pour le client Linux Ubuntu 22.04 LTS :

- Nom :  CLILIN02
- Même compte avec même mot de passe
- Adresse IP fixe : 172.16.10.30/24

### **5. Difficultés rencontrées**

Projet initial _Zulip_

* Problème de communication entre les sources sur le réseau local

* Problème d'installation de _Zulip_ côté serveur

* Difficultes de configuration de _Zulip_ sur le serveur

* Problème lors de l'ajout d'utlisateur (uniquement par mail)

* Ajout serveur mail pour palier aux problèmes d'ajout utlisateur (solution infructueuse)

Projet **_Rocket.Chat_**

* Difficultés à l'installation en lien avec la configuration matérielle

### **6. Solutions et/ou Alternatives trouvées pour palier aux problèmes**

Projet initial _Zulip_

* Modification du fichier settings.py pour configurer le serveur

Projet **_Rocket.Chat_**

* Problème d'installation résolu en forcant l'installation avec une version précédente (voir FAQ INSTALL.md)

Suite à tous les problèmes rencontrés côté serveur et principalement celui concernant l'ajout des utilisateurs, l'équipe du projet, en lien avec le partenaire, a par conséquent opté pour changer de logiciel de messagerie.

Après analyse et concertation avec le partenaire, il apparait que **_Rocket.Chat_** est la solution la plus viable.

Ce choix capital n'a en aucun cas remis en cause la Deadline du projet. L'équipe en charge du projet a redoublé d'efforts pour rendre un produit d'exception.

### **7. Next-Step : Améliorations possibles envisagées**

Il est possible de rajouter des modules à **_Rocket.Chat_**, ceux-ci sont variés, l'ensemble des modules sont disponibles sur _MarketPlace_ interne de **_Rocket.Chat_**
Il appartient à ladministrateur du serveur d'adapter ces modules en fonction des besoins de l'organisation

A titre d'exemple, les modules **ChatGPT**, **GitHub**, **Drive** (de Google), **Twitter**, **WhatsApp** sont disponibles.
