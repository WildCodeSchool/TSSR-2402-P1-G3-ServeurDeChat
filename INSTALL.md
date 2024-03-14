# Implémentation d'un serveur de messagerie instantanée (chat)

![Zulip](attachments/Zulip.png)

Ce document est réservé à usage interne, il ne peut en aucun cas être divulgué à des tiers.

Dernière mise à jour du Document : **14 mars 2024**

## **Sommaire**

1. Pré-requis techniques

2. Installation et Configuration : Les étapes pas à pas

3. FAQ

## **1. Pré-requis techniques**

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

Le Serveur est sous Debian 12.5.

Pour le serveur Debian 12.5 :
- Nom : SRVLX01
- Compte : root
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.10/24

## **2. Installation et Configuration : Step by Step**

### **Installation sur le serveur Debian SRVLX01**

### **Installation sur les clients**

#### **Installation sur le Client Ubuntu CLILIN01**

Une fois connecté au Client Linux, ouvrez le Terminal de commande.

Il vous faut dans un premier temps installer _snap_ sur votre client.

```
sudo apt update
sudo apt install snapd
```

Vous pouvez ensuite procéder à l'installation de _zulip_ via la commande.

```
sudo snap install zulip
```

Vous pourrez démarrer Zulip :
* Depuis le menu des applications Ubuntu
* Depuis le terminal via la commande `zulip`

Le logiciel de messagerie **Zulip** est désormais installé et opérationnel pour l'utilisateur. Il restera toutefois à l'utilisateur d'effectuer la configuration lors de sa première connexion (voir USER_GUIDE.md).

#### **Installation sur le Client _Windows CLIWIN02_**

Depuis le Client Windows, rendez-vous sur la page de téléchargement de Zulip : [Download Zulip for Windows](https://zulip.com/apps/).

Téléchargez l'éxécutable et lancez-le pour installer le logiciel sur le Client.

Lors de l'instalation, sélectionnez les options suivantes :

Sélectionnez _Pour tous ceux qui utilisent l'ordinateur (tous les utilisateurs)_ puis cliquez sur _Suivant_.

![Zulip_Install_Win_01](attachments/Zulip_Install_Win_01.jpg)

NB. Ainsi, tous les utilisateurs ayant accés à ce Client pourront bénéficier de l'expérience de Zulip.

Autorisez l'application à apporter des modifications à votre appareil.

![Zulip_Install_Win_02](attachments/Zulip_Install_Win_02.jpg)

Laissez le dossier de destination par défaut : `C:\Program Files\Zulip` puis cliquez sur _Installer_.

![Zulip_Install_Win_03](attachments/Zulip_Install_Win_03.jpg)

Une fois l'installation terminée, vous pouvez quitter en cliquant sur _Fermer_, il n'est pas obligatoire de lancer Zulip à la fin de l'installation.

![Zulip_Install_Win_03](attachments/Zulip_Install_Win_04.jpg)

Le logiciel de messagerie **Zulip** est désormais installé et opérationnel pour l'utilisateur. Il restera toutefois à l'utilisateur d'effectuer la configuration lors de sa première connexion (voir USER_GUIDE.md).

## **3. FAQ**
