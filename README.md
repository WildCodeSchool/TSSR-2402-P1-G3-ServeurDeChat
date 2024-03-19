# **Implémentation d'un serveur de messagerie instantanée (chat)**

![RocketChat](attachments/rocketchat_original.png)

Ce document est réservé à usage interne, il ne peut en aucun cas être divulgué à des tiers.

Dernière mise à jour du Document : **19 mars 2024**

## **Sommaire**

1. Présentation du projet et objectifs finaux

2. Introduction : Mise en contexte

3. Présentation des membres du groupe et de leur rôles

4. Choix techniques et contraintes

5. Difficultés rencontrées

6. Solutions et/ou Alternatives trouvées pour palier aux problèmes

7. Next-Step : Améliorations possibles envisagées

### **1. Présentation du Projet et Objectifs finaux**

Le projet consiste à installer le software **_RocketChat_** sur notre Serveur Debian, afin que celui-ci donne accés à toutes les fonctionnalités qu'offre le logiciel sur nos 2 ordinateurs Clients (Ubuntu et Windows).

La Deadline du projet est fixée au **vendredi 22 mars 2024**.

Une présentation de l'avancement du projet sera effectué le vendredi 15 mars 2024.

A l'issue du projet, les services devront être opérationnels et stables.

La documentation doit impérativement être jointe une fois le projet abouti, elle seras rédigée sous format markdown et comprendras :

- une documentation générale (README.md)
- une documentation administrateur (INSTALL.md)
- une documentation utilisateur (USER_GUIDE.md)

Un dépôt GitHub a été créé à cet effet : [TSSR-2402-P1-G3-ServeurDeChat](https://github.com/WildCodeSchool/TSSR-2402-P1-G3-ServeurDeChat)

Il est demandé dans un second temps, suivant l'avancée du projet de procéder à la personnalisation des emojis et des réactions selon les conversations.
Ceci n'est pas une priorité, cette partie pourra être intégré lors d'un Next-Step.

### **2. Introduction : Mise en contexte**

Le projet devrait faciliter grandement la communication entre nos collaborateurs, et permettras ainsi d'avancer avec plus d'efficacité sur les projets en cours.

### **3. Présentation des membres du groupe et de leur rôles**

Le Projet **RocketChat** est composé des membres de la DSI :

* **Anaïs Lenglet**
* **Pierre Girard**
* **Julien Guillot**
* **Yanis Hortholary**
* **Anthony Javault**

Rappel des rôles et responsabilités :

- Rôle du _Scrum Master_ (SM) :

    > Le SM est le garant de la bonne application de la méthode Scrum. Il est responsable de la communication entre les membres de l'équipe et de la bonne réalisation des tâches.
            
- Rôle du _Product Owner_ (PO) :

    > Le PO est le représentant du client. Il est responsable de la définition des besoins et de la priorisation des tâches. Il est le garant de la qualité du produit final.
            
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
|Configuration des Clients|||x|x||
|Tests Serveur||x|x|||
|Tests Clients||||x|x|
|Documentation|x||||x|




### **4. Choix techniques et contraintes**

En ce qui concerne la version serveur, **RocketChat** étant plus otptimisé pour Debian, le choix est évident.

Le Serveur est par conséquent sous Debian 12.5 :
- Nom : SRVLX01
- Compte : root
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.10/24

Les clients sont respectivement sous OS Windows 10 (client 1) Ubuntu 22.04 LTS (client 2).

Pour le client Windows 10 : 
- Nom : CLIWIN01
- Compte utilisateur : wilder (dans le groupe des admins locaux)
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.20/24

Pour le client Ubuntu 22.04 LTS :
- Nom :  CLILIN02
- Même compte avec même mot de passe
- Adresse IP fixe : 172.16.10.30/24

### **5. Difficultés rencontrées**

Projet initial **Zulip**

* Problème de communication entre les sources sur le réseau local

* Problème d'installation de Zulip côté serveur

* Difficultes de configuration de Zulip sur le serveur

* Problème lors de l'ajout d'utlisateur (uniquement par mail)

* Ajout serveur mail pour palier aux problèmes d'ajout utlisateur (solution infructueuse)

### **6. Solutions et/ou Alternatives trouvées pour palier aux problèmes**

Projet initial Zulip

* Modification du fichier settings.py pour configurer le serveur

Suite à tous les problèmes rencontrés côté serveur et principalement celui concernant l'ajout des utilisateurs, l'équipe du projet en lien avec le partenaire a par conséquent opter pour changer de logiciel de messagerie.
Il apparait que RocketChat serait la solution la plus viable.

Ce choix ne remet nullement en cause la Deadline du projet. L'équipe en charge du projet redoubleras d'efforts pour rendre un produit d'exception.


### **7. Next-Step : Améliorations possibles envisagées**