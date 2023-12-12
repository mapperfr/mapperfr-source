---
title: Git, Gitlab, Github... Qu'ès aco?
summary: ''
authors: [Jérémy Garniaux]
tags: [git, gitlab, github, vcs]
categories: []
date: "2023-12-11"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # white, black, league, beige, sky, night, serif, simple, solarized
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
  reveal_options:
   transition: 'none'
---

### Git, Gitlab, Github... Qu'es aquò?

Introduction à la journée "Explorer le potentiel de Git et Gitlab"  
12 décembre 2023  
MMSH

![](albums/slides/git/bandeau.png)

{{< speaker_note >}}

Bonjour et merci pour votre présence à cette journée d'atelier sur Git et Gitlab proposée par la mission Humanités numériques et le Pôle édition de la MMSH. La journée est accessible in vivo et en visio - je crois d'ailleurs qu'un enregistrement est prévu si ça convient à tout le monde. La matinée sera consacrée à des retours d'expérience d'utilisateurs de Git dans des contextes d'Humanités numériques, tandis que l'après-midi prendra une forme plus participative avec un atelier pratique où l'on pourra approcher concrètement Git à travers l'interface web qu'est Gitlab.

{{< /speaker_note >}}

---

#### Git, Gitlab, Github... Qu'es aquò?

{{% fragment %}} - Historique et usages de Git {{% /fragment %}}  
{{% fragment %}} - Ligne de commande et interfaces graphiques {{% /fragment %}}  
{{% fragment %}} - Interfaces web (partiellement commerciales): les forges {{% /fragment %}}  

{{< speaker_note >}}

J'ai été invité à ouvrir la journée en tentant de répondre à une première question: de quoi parle-t-on? Git, Github, Gitlab, voire Gitea ou encore Codeberg -- qu'es aquò? Comme on dit ici. Pour tenter d'y répondre en une petite demi-heure, je tracerai un rapide historique de Git, cet outil décentralisé de gestion de version et je présenterai ensuite ses différentes interfaces qui sont comme autant de portes d'accès - que ce soit "en local" sur ma machine avec la ligne de commande ou un "client graphique", c'est à dire un logiciel disposant d'une interface graphique, mais aussi des interfaces disponibles sur le web, comme Github et Gitlab, qui en plus des fonctionnalités du logiciel Git, proposent des fonctionnalités de partage de code (dépôts publics), de réseau social (avec des abonnés et des abonnements), de wikis, d'outils de gestion de projet, etc.

{{< /speaker_note >}}

---

#### Git, Un logiciel libre de gestion de version décentralisé

{{% fragment %}} - Libre et gratuit, créé en 2005 par Linus Torvalds {{% /fragment %}}  
{{% fragment %}} - Permet de stocker un ensemble de fichiers en conservant la chronologie des modifications effectuées dessus  {{% /fragment %}}  
{{% fragment %}} - Décentralisé: système de connexion pair à pair {{% /fragment %}}  
{{% fragment %}} - Pour du code, mais pas seulement! Livres, articles... {{% /fragment %}}  
{{% fragment %}} - Un outil d'abord disponible en ligne de commande {{% /fragment %}}  

{{< speaker_note >}}

Git est un logiciel libre de gestion de version décentralisé. 

- Logiciel libre, librement reproductible, distribuable, etc. créé en avril 2005 par Linus Torvalds, développeur finlandais (maintenant américain), et dont le développement est mené, depuis, par le Japonais Junio Hamano et l'américain Jeff King. Git a été créé à l'origine pour remplacer un programme propriétaire, _BitKeeper_. 

Ce dernier - qui était alors gratuit mais pas libre ni ouvert - était utilisé pour le développement du noyau Linux. Lorsqu'Andrew Tridgell, développeur à l'ODSL (future Fondation Linux), tente la rétro-ingénierie de certains protocoles de BitKeeper (= comprendre le fonctionnement d'un système fermé en le devinant), ce statut gratuit est révoqué, ce qui pousse Linus Torvalds à créer Git pour se défaire de BitKeeper. 

- Logiciel de gestion de version: il permet de _stocker un ensemble de fichiers en conservant la chronologie des modifications effectuées dessus_, et de retrouver au besoin un état précédent d'un fichier.
- Il est décentralisé: il ne repose pas sur un serveur central mais utilise un système de connexion pair à pair.

Il est principalement utilisé en développement logiciel, lorsque les fichiers concernés contiennent du code informatique, mais peut être utilisé avec d'autres types de projets. Des rédactions collaboratives d'ouvrages ou d'articles on été menées en utilisant Git. 

Git est d'abord un outil disponible via une interface en ligne de commande. La ligne de commande, c'est cette interface textuelle accessible en général à l'aide d'un terminal qui permet de donner des instructions à l'ordinateur, qui va les éxécuter, avant d'afficher un retour - réussite ou échec de la commande, texte d'aide, description du contenu d'un dossier, etc.

Pour utiliser Git, on se déplace dans le dossier où l'on veut travailler, puis on tape la commande `git` suivie d'un ou plusieurs autres termes. Ces commandes permettent d'assurer un certain nombre de fonctionnalités.

{{< /speaker_note >}}

---

#### Fonctionnalités

- Créer un nouveau dépôt et surveiller les fichiers présents dans un dossier: `git init`  
- Ajouter les fichiers récemment modifiés à la liste des fichiers surveillés: `git add`  
- Valider cet ajout: `git commit`  
- créer ou gérer différentes branches dans le code: `git branch`  
- fusionner des branches: `git merge`  

{{< speaker_note >}}

La notion très importante c'est celle de commit: lorsqu'on "commit", on crée un instantané, ou une "version", de l'état du code. Lorsqu'on veut revenir à une version précédente du code, on restaure tel ou tel commit. 

{{< /speaker_note >}}

---

#### Fonctionnalités

- Clone (=copier) en local un dépôt distant: `git clone`  
- Récupérer le code le plus à jour sur un dépôt distant: `git pull`  
- Publier des révisions ou contributions sur un dépôt distant: `git push`  
- Défaire les modifications d'un _commit_ précédent: `git revert`  
- Etc.

{{< speaker_note >}}

Il y a ensuite la notion de dépôt distant - on reviendra dessus dans un instant, lorsqu'on parlera de Github ou de Gitlab.

{{< /speaker_note >}}

---

#### De nombreuses interfaces graphiques disponibles 

{{% fragment %}} git-gui, gitk, {{% /fragment %}}  
{{% fragment %}} TortoiseGit, Git Extensions, Magit, MeGit, GitUp, gitg, ungit, Fugitive, Guitar, git-cola, GitGUI, giggle, RepoZ, Gitgui, Gittyup, Git Klient, gitonic, Gitnuro, Pragma-git... {{% /fragment %}}  

{{< speaker_note >}}

En plus de l'interface de base en ligne de commande, le projet de base propose deux interfaces graphiques, git-gui (pour effectuer des `commit`) et gitk (pour parcourir le code et les commits qui l'ont affecté). De nombreuses interfaces graphiques tierces ont été créées au fil des années. Le site internet de Git en propose une liste, dont je reprends ici uniquement les exemples sous licence libre - il y en a au moins autant sous licence propriétaire, et pour les trois principales plateformes, Windows, Mac ou Linux. On a donc l'embarras du choix pour travailler avec Git en local. 

{{< /speaker_note >}}


--- 

#### De nombreuses interfaces disponibles 

![](albums/slides/git/gitg.png)  
 https://git-scm.com/downloads/guis

---

#### L'apparition des forges logicielles en ligne

{{% fragment %}} - De la gestion de version à la forge: des interfaces web enrichies {{% /fragment %}}  
{{% fragment %}} - 2008: Github {{% /fragment %}}  
{{% fragment %}} - 2011: Gitlab {{% /fragment %}}

{{< speaker_note >}}

Git rencontre très vite un grand succès et de nouvelles interfaces enrichies apparaissent sous la forme de forges logicielles. Présentée sous la forme d'un site internet, une forge peut proposer, en plus des fonctions de gestion de versions du code: 
- des gestionnaire de listes de diffusion;
- des outils de suivi de bugs;
- des gestionnaires de documentation de type wiki;
- des outils de gestion des tâches;
- des outils de traduction en ligne;
- La possibilité de présenter son projet avec une page d'accueil;
- la publication régulière d'actualités relatives à son projet.

Tout ceci dans une interface intégrée, enrichie de fonctionnalités proches de celles des réseaux sociaux (compte utilisateur public, abonnés et abonnements, mise en favori de projets).

Les forges facilitent le travail collaboratif autour d'un dépôt commun de code, et intègrent des outils de plus en plus spécifiques.

La forge la plus célèbre, Github.com, est lancée en 2008. En 2012, elle compte près de 3 millions d'utilisateurs et près de 5 millions de dépôts. En 2018, Github est rachetée par Microsoft, ce qui provoque une certaine inquiétude quant à son positionnement et son avenir (et une fuite toute relative des projets - dans la journée, 50 000 projets migrent vers Gitlab, c'est beaucoup, ce n'est pas tant). En 2023, Github continue d'être la forge la plus active, de loin, et compte plus de 100 millions d'utilisateurs. 

Gitlab, de son côté, est créé en 2011. Si les fonctionnalités proposées par Gitlab sont proches de celles de Github, son fonctionnement est un peu différent: en plus de la forge proposée à l'adresse Gitlab.com, Gitlab propose deux version (CE et EE -- la forge disponible sur Gitlab.com est basée sur l'EE) que l'on peut installer sur le serveur de son choix. C'est le modèle économique de l'open core, avec une version de base proposée en open source et des versions complémentaires enrichies de fonctionnalités.

{{< /speaker_note >}}

------

#### Gitlab

{{% fragment %}} - Intégration continue + déploiement et/ou livraison continue (CI/CD), DevOps {{% /fragment %}}  
{{% fragment %}} - Plusieurs instances existantes, et possibilité de déployer sa propre instance {{% /fragment %}}   

{{< speaker_note >}}

Gitlab est donc une forge logicielle en ligne, basée sur Git, et qui propose les fonctionnalités complémentaires que je viens de décrire. Elle se spécialise également sur des outils dits d'intégration continue et de livraison ou de déploiement continu (CI/CD): 

- CI: Chaque modification (commit) est testée automatiquement pour éviter de casser l'existant
- CD: Livraisons ou déploiement du code rapides et automatisées. (Livraison = le code est partagé dans le dépôt principal de la forge. Déploiement = le code est mis en production, qu'il s'agisse d'un site web ou d'un logiciel).

Gitlab se présente souvent comme une plateforme de "DevOps". Le DevOps est une approche qui propose d'unifier le développement logiciel et l'administration des infrastructures informatiques. Je le cite pour info car c'est un élément souvent mis en avant concernant Gitlab mais ce n'est pas d'une importance capitale ici. 

La particularité de Gitlab, comme je vous le disais plus tôt, c'est de proposer la possibilité d'installer une instance du logiciel sur un serveur de son choix. C'est ce qu'a fait Huma-Num, qui propose une instance à https://gitlab.huma-num.fr. 

{{< /speaker_note >}}

------

#### Gitlab

https://gitlab.com  
https://gitlab.huma-num.fr  
https://gitlab.gnome.org   
https://gitlab-forge.din.developpement-durable.gouv.fr  
https://gitlab.depp.education.fr  

etc!

{{< speaker_note >}}

C'est aussi le cas de la fondation Gnome (environnement de bureau sous Linux), de plusieurs ministères, de l'IGN, etc.

Ces instances sont bien distinctes du site Gitlab.com!

{{< /speaker_note >}}

------

#### Git et Gitlab pour OrAG

Suivi des versions du code en local  
Dépôt pour l'instant privé  
https://gitlab.huma-num.fr  

On explore!

{{< speaker_note >}}

Après cette introduction un peu verbeuse, je vous propose de vous présenter rapidement comment j'utilise Git et Gitlab dans le cadre du projet OrAG. C'est une utilisation a minima de la forge logicielle: ce sont surtout les fonctionnalités de Git qui m'importent ici, pour conserver l'historique des versions de mes fichiers. Le projet Gitlab est pour l'instant en statut privé; lorsque OrAG sera livré, nous pourrons basculer le projet en statut public pour que le code soit véritablement open source.

Manip: présentation du projet en local et sur Gitlab, modification d'un fichier, add/commit/push, nouveau tour, puis modification en ligne via l'éditeur intégré,e tC.

{{< /speaker_note >}}

------

#### Merci pour votre attention!

Jérémy Garniaux  
jeremy.garniaux@univ-amu.fr 

![](albums/slides/git/bandeau.png)

