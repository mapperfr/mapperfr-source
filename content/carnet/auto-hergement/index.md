---
title: L'auto-hébergement, un an après
author: Jérémy Garniaux
type: post
date: 2022-03-09
categories:
  - carnet
tags:
  - yunohost
  - sysadmin
  - linux
  - serveur
  - auto-hébergement
draft: true
---

Spoiler: j'ai désinstallé le serveur.

## Ma problématique de départ
Installer un serveur à la maison pour disposer:
- D'ne instance de Nextcloud pour synchroniser mes données entre mon laptop personnel et celui du taf
- D'un espace serveur pour déployer mon site personnel, alors basé sur Wordpress

## Yunohost
Yunohost était une solution intéressante: permet de s'initier à l'admin serveur progressivement. 

J'ai ajouté ensuite des services "bonus" auxquels je ne pensais pas au départ: un serveur mail, et divers services: un lecteur de flux RSS, une appli de lecture "plus tard" (wallabag)...

- Présentation de Yunohost

- 9 topics lancés sur le forum Yunohost: 4 dans le premier mois, deux dans le mois suivant, deux au fil de l'eau, dans l'année, et un dernier ayant mené à la désinstallation du serveur. 

### Le lancement


- Premier problème [avec l'hébergeur précédent de mon site personnel, o2switch](https://forum.yunohost.org/t/dns-server-info-not-records-server/13665/5). Incompréhension sur ma démarche et la nécessité d'éditer les DNS pour renvoyer sur Yunohost. J'ai demandé la portabilité et migré mon nom de domaine vers Gandi. 
- Second problème: [Nginx meets Wordpress](https://forum.yunohost.org/t/weird-redirection-on-a-custom-web-app-wordpress-install-after-changing-the-app-url/13815/6). J'ai découvert à mes dépens que les deux ne sont pas très compatibles, surtout si l'on souhaite afficher de "belles URLs" (_pretty URLs_) dans Wordpress. J'ai perdu pas mal de temps avant de comprendre comment paramétrer nginx.conf. Ça a fonctionné pendant un moment, jusqu'aux bugs finaux. J'y reviendrai. 
- Troisième demande d'assistance: [Les joies de Let's Encrypt](https://forum.yunohost.org/t/erreur-www-lets-encrypt/13833). Où je découvre que http://mapper.fr et http://www.mapper.fr ne sont pas la même adresse, que cet anodin www est une autre adresse. 
- [OpenOffice](https://forum.yunohost.org/t/onlyoffice-fails-to-install/13948). OnlyOffice en tant qu'app intégrée à Nextcloud n'est pas compatible avec les processeurs ARM - donc avec le Raspberry Pi. Et je n'ai pas réussi à installer Collabora Online, la version cloud de LibreOffice.

### Passer la seconde

- Une petit coup de pouce de la communauté pour [déplacer mes données sur un disque externe](https://forum.yunohost.org/t/deplacement-donnees-nextcloud-sur-disque-externe-erreur-au-scan-du-nouveau-repertoire/14440/3). Pas top d'installer Nextcloud sur une carte SD! (LIEN?)

### Conclusion 

Auparavant, malgré des années à mettre en place des sites personnels successifs reposant sur des hébergements loués, et n'ayant pas de formation ni de besoin professionnel dans le domaine, la cuisine interne de l'administration serveur (DNS, permissions, accessibilité réseau...) était restée une inaccessible boîte noire. Ce temps passé sur Yunohost m'a permis de clarifier beaucoup de points et de me sentir beaucoup plus à l'aise. Je n'exclus pas d'y revenir plus tard!