# **Implémentation d'un serveur de messagerie instantanée (chat)**

Ce document est réservé à usage interne, il ne peut en aucun cas être divulgué à des tiers.

Dernière mise à jour du Document : **11 mars 2024**

## **Sommaire**

1. Présentation du projet et objectifs finaux

2. Introduction : Mise en contexte

3. Présentation des membres du groupe et de leur rôles

4. Choix techniques et contraintes

5. Difficultés rencontrées

6. Solutions et/ou Alternatives trouvées pour palier aux problèmes

7. Next-Step : Améliorations possibles envisagées

### **1. Présentation du Projet et Objectifs finaux**

    Objectif principal :
    Mettre en place un serveur de messagerie instantanée (chat) 
    Le logiciel Zulip doit être utilisé
    Serveur : Debian 12
    Client : tous les OS client sont utilisable (il faut 2 clients)

    Objectif secondaire :
    Personnalisation des emojis et des réactions selon les conversations


Les livrables sont les résultats ou les produits finaux du projet qui sont livrés au client ou aux parties prenantes.
Ils peuvent inclure rapports, documents, logiciels, etc.

Ils sont disponibles sur la plateforme GitHub, un dépôt a été créé à cet effet : [TSSR-2402-P1-G3-ServeurDeChat](https://github.com/WildCodeSchool/TSSR-2402-P1-G3-ServeurDeChat)

### **2. Introduction : Mise en contexte**

### **3. Présentation des membres du groupe et de leur rôles**

Le Projet **Zulip** est composé de :

* **Anaïs Lenglet**
* **Pierre Girard**
* **Julien Guillot**
* **Yanis Hortholary**
* **Anthony Javault**

Rôle du _Scrum Master_ (SM) :

> Le SM est le garant de la bonne application de la méthode Scrum. Il est responsable de la communication entre les membres de l'équipe et de la bonne réalisation des tâches.
            
Rôle du _Product Owner_ (PO) :

> Le PO est le représentant du client. Il est responsable de la définition des besoins et de la priorisation des tâches. Il est le garant de la qualité du produit final.
            
Sont nommés pour la première semaine de Projet (Sprint 1) :

* PO : **Julien Guillot**
* SM : **Yanis Hortholary**
            
Sont nommés pour la seconde semaine de Projet (Sprint 2) :

* PO : **thsh**
* SM : **dyhjhjd**

Attribution des tâches/activités par membre :

|Activités|**Anaïs Lenglet**|**Pierre Girard**|**Julien Guillot**|**Yanis Hortholary**|**Anthony Javault**|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Mise en place et configuration du Serveur|
|Mise en place et configuration des Clients|
|Tests Serveur / Client|
|Documentation|




### **4. Choix techniques et contraintes**

Les clients sont respectivement sous OS Windows 10 (client 1) Ubuntu 22.04 LTS (client 2).

Pour le client Windows 10 : 
Nom : CLIWIN01
Compte utilisateur : wilder (dans le groupe des admins locaux)
Mot de passe : Azerty1*
Adresse IP fixe : 172.16.10.20/24

Pour le client Ubuntu 22.04 LTS :
Nom :  CLILIN02
Même compte avec même mot de passe
Adresse IP fixe : 172.16.10.30/24

Le Serveur est sous Debian 12.5.

Pour le serveur Debian 12.5 :
Nom : SRVLX01
Compte : root
Mot de passe : Azerty1*
Adresse IP fixe : 172.16.10.10/24



### **5. Difficultés rencontrées**

### **6. Solutions et/ou Alternatives trouvées pour palier aux problèmes**

### **7. Next-Step : Améliorations possibles envisagées**
