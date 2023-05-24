---
title: Utiliser Walking Papers pour cartographier dans OpenStreetMap
author: Jérémy Garniaux
type: post
date: 2009-12-09T13:15:11+00:00
draft: false
categories:
  - tutos
tags:
  - JOSM
  - openstreetmap
  - Potlatch
  - tuto
  - Walking Papers

---

Walk­ing Papers est un ser­vice qui per­met de con­tribuer à OpenStreetMap sans dis­pos­er de GPS. Si cer­tains procédés exis­tent déjà qui per­me­t­tent de car­togra­phi­er sans GPS (en se reposant notam­ment sur les pho­tos aéri­ennes de Yahoo ou le cadas­tre français), il s’ag­it à ma con­nais­sance de la pre­mière méth­ode autorisant la car­togra­phie de ter­rain sans GPS. Comme je n’en avais pas moi-même, j’ai testé ce Walk­ing Papers avec une cer­taine curiosité, et voilà donc un petit compte-ren­du / tuto­riel de l’opération!

## Wolquine pèpeure ?

Le principe de Walk­ing Paper est sim­ple. Il s’ag­it d’im­primer un extrait d’Open­StreetMap sur une feuille A4; d’aller ensuite sur le ter­rain ren­seign­er tous les élé­ments exis­tants mais absents de la base de don­nées, en les dessi­nant sur la feuille et en prenant des notes sup­plé­men­taires si néces­saire; enfin, une fois de retour, et après avoir scan­né la carte de ter­rain, de s’en servir comme guide pour reporter dans OSM tous ces nou­veaux élé­ments en les tag­gant comme il se doit.

## Le ter­ri­toire

La zone que j’ai choisi de car­togra­phi­er se situe à Saint-Quentin-en-Yve­lines, au croise­ment des com­munes de Guyan­court, Mag­ny-les-Hameaux et Voisins le Bre­ton­neux. Voilà ce qu’af­fiche Open­StreetMap avant le pas­sage:

[![OSM_st_quentin_avant](albums/carnet/walking_papers/osmstquentin_avant.png)

C’est l’espace situé entre la route de Chateau­fort, l’av­enue de l’Eu­rope et la D91, rel­a­tive­ment peu ren­seigné, que j’ai choisi d’aller cartographier.


## Impres­sion de la carte

La [page d’ac­cueil du site Walk­ing Papers](https://walking-papers.org/#make) per­met de définir la zone qu’on souhaite imprimer :

[![print_st_quentin](albums/carnet/walking_papers/print_st_quentin.png)

Comme l’indique le site, un niveau de zoom d’au moins 14 est néces­saire pour éviter de se retrou­ver avec des zones trop grandes (et donc peu pré­cis­es). En fonc­tion des besoins, il est pos­si­ble de con­fig­ur­er l’af­fichage en por­trait ou en paysage. Une fois le cadrage effec­tué, un clic sur “Make” nous amène à une page d’où l’on peut télécharg­er le “Walk­ing Paper” pour impression :

[![print_st_quentin_pret](albums/carnet/walking_papers/print_st_quentin_pret.png)

Il n’y a plus qu’à imprimer et à aller se balad­er… En plus de not­er tous les élé­ments absents de la carte d’o­rig­ine, on prof­it­era de la sor­tie pour véri­fi­er ce qui est déjà car­tographié, notam­ment les noms de rues.

## Ren­voy­er la carte sur les serveurs de Walk­ing Papers après le terrain

Voilà à quoi ressem­blait ma carte une fois re-scannée :

![Walking Paper 3](albums/carnet/walking_papers/walkingpapers3.jpg)

C’est surtout le quart nord-ouest de la zone que j’ai ren­seigné. Comme je dis plus haut, il s’ag­it d’un espace partagé par trois com­munes, espace dédié aux activ­ités ter­ti­aires et au rési­den­tiel. Dans la moitié sud de la carte, il existe en réal­ité un lotisse­ment assez impor­tant ; j’ai com­mencé à le dessin­er avant de me ravis­er, les faux angles droits des rues étant au-delà de mes capac­ités de “car­tographe à main lev­ée”. J’ai donc préféré atten­dre de con­sul­ter le cadas­tre pour inté­gr­er cette zone à OSM.

Mais avant de pou­voir éditer Open­StreetMap sur la base des infor­ma­tions récoltées ici, plusieurs étapes sont néces­saires : scan­ner la carte papi­er, d’abord, puis ren­voy­er ce scan sur les serveurs de Walk­ing Papers.

Cette étape peut pos­er prob­lème: j’ai du essay­er de nom­breuses fois avant que ça fonc­tionne pour cette carte. Si ça ne fonc­tionne pas mal­gré une bonne con­fig­u­ra­tion (au moins 200 dpi, et le QRcode sur le côté droit), c’est qu’il vaut mieux atten­dre un peu et rées­say­er plus tard…

Une fois envoyée, la carte est recalée automa­tique­ment. Cette réin­té­gra­tion du scan final est pos­si­ble grâce au croise­ment de [deux tech­niques dif­férentes](https://mike.teczno.com/notes/walking-papers.html) : [SIFT](https://people.cs.ubc.ca/%7Elowe/keypoints/) d’un côté, qui per­met la recon­nais­sance des formes présentes autour de la carte (la main avec le sty­lo par exem­ple) pour déter­min­er le sens de lec­ture, et un [QR Code](https://fr.wikipedia.org/wiki/Code_QR) de l’autre pour indi­quer les coor­don­nées géo­graphiques de la carte.

## L’édi­tion

Deux modes d’édi­tion sont pos­si­bles : l’un directe­ment dans Pot­latch, le sec­ond dans JOSM à l’aide d’un plu­g­in Walk­ing Papers (voir le wiki OSM pour des détails sur l’u­til­i­sa­tion des deux logi­ciels). Le choix de l’édi­teur ren­voie aux choix de cha­cun : Pot­latch — l’édi­teur en ligne — est plus facile d’usage, mais est assez gour­mand en ressources (il m’ar­rive de faire planter Fire­fox en édi­tant dans Pot­latch, avec 2 Go de RAM sur le PC…). Voilà à quoi ressem­ble Pot­latch si on l’ou­vre depuis la page “Scans” de Walk­ing Papers :

![Edition Potlatch](albums/carnet/walking_papers/potlatch.png)

On voit que par-dessus la carte papi­er se super­posent les voies et nodes actuelle­ment présents dans OSM. C’est égale­ment le cas avec JOSM : pour pou­voir affich­er le Walk­ing Paper dans ce dernier, il faut installer le [plu­g­in Walk­ing Papers](https://wiki.openstreetmap.org/wiki/JOSM/Plugins/WalkingPapers), qui aura besoin du numéro de la carte pour l’af­fich­er (ce numéro est lis­i­ble à la fin de l’URL de la page de la carte que l’on vient de ren­voy­er sur le site de WP). La super­po­si­tion de la carte de ter­rain et des élé­ments OSM présents dans la zone donne quelque chose comme ça :

[![edition=josm](albums/carnet/walking_papers/edition_josm.png)

Le tra­vail de car­togra­phie peut ensuite se faire, en s’aidant des infor­ma­tions présentes sur le Walk­ing Paper. À vous de jouer!