---
title: Mapstodon.space, une instance Mastodon pour la communauté des cartographes
author: Jérémy Garniaux
type: post
date: 2009-01-09T14:04:19+00:00
draft: true
categories:
  - carnet
tags:
  - mastodon
  - twitter
  - activitypub
  - fediverse
---

Depuis le rachat et la reprise chaotique de Twitter par Elon Musk, entre choix contestés, licenciements massifs et erreurs d'appréciation, un nombre croissant de ses utilisateurices fuient le réseau. Certaines ont fermé leur compte définitivement, d'autres le désactivent, d'autres encore (comme moi) y ralentissent fortement leur activité. L'occasion fait le larron: le côté toxique de Twitter prend le pas depuis un certain temps sur ses aspects les plus enrichissants. Pour beaucoup, nourris par de nombreux échanges riches et respectueux, nous y restions en esquivant au mieux ses aspects les plus pénibles: l'opacité de l'algorithme qui décide à notre place du contenu auquel on accède, l'incitation permanente au conflit *par dessein* [^1] ("l'engagement", qu'ils disaient), l'analyse du trafic via le raccourcisseur d'URL, etc. 

Une partie de ce beau monde cherche donc une nouvelle maison pour continuer la conversation.

## Introducing Mastodon

Une alternative libre, décentralisée et interopérable à Twitter existe depuis 2016, [Mastodon](https://en.wikipedia.org/wiki/Mastodon_(software)). 
- Libre: le code source de Mastodon [est publiée sur Github](https://github.com/mastodon/mastodon) sous licence AGPLv3+.
- Décentralisée: Contrairement à Twitter, Mastodon ne dépend pas d'un fournisseur de service unique. Il prend la forme d'un ensemble d'instances (ou serveurs), administrées séparément. Cet aspect demande un temps d'adaptation lorsqu'on arrive du web centralisé et d'une plateforme comme Twitter. L'analogie avec l'email [^2] peut faciliter la compréhension dans les premiers temps.
- Interopérable: Mastodon repose sur [ActivityPub](https://fr.wikipedia.org/wiki/ActivityPub), un format standard d'échanges, ouvert, interopérable et documenté. Il est implémenté par un ensemble de logiciels et de services: Peertube (hébergement et consultation de vidéos) ou bien Pixelfed (alternative libre à Instagram), par exemple, sont d'autres logiciels implémentant ActivityPub. La migration en cours d'utilisateurs de Twitter vers Mastodon [semble avoir relancé l'intérêt pour ActivityPub](https://thenewstack.io/devs-are-excited-by-activitypub-open-protocol-for-mastodon/). Tumblr [a indiqué](https://techcrunch.com/2022/11/21/tumblr-to-add-support-for-activitypub-the-social-protocol-powering-mastodon-and-other-apps) qu'il intégrerait prochainement le standard. 

Au-delà de l'aspect technique du protocole d'échange qu'il partage avec d'autres outils, Mastodon s'inscrit dans le vaste mouvement de [la Fédiverse](https://fr.wikipedia.org/wiki/Fediverse), fédération de services libres et ouverts pensés et conçus en alternative aux réseaux sociaux fermés et commerciaux. La Fédiverse est une très belle boîte de Pandore qui dispose de plusieurs portes d'entrée - je vous invite à pousser celle de https://fediverse.party pour en découvrir plus. 

## Introducing MaPstodon

Enthousiasmé par Mastodon, j'avais créé un premier compte il y a un certain temps, remplacé au printemps 2020 (pendant le premier confinement) par un second sur [mamot.fr](https://mamot.fr), serveur mis à disposition par l'association [la Quadrature du Net](https://www.laquadrature.net/). Fin octobre, l'activité s'est brusquement intensifiée sur Mastodon, tandis que sur Twitter, les conversations se multipliaient - avec cette question récurrente: "sur quelle instance m'inscrire?" - car la multiplication des instances, malgré des outils d'aide au choix comme https://joinmastodon.org, ne semblait pas faciliter l'adoption.

Comment faciliter ou encourager, à mon niveau, cette joyeuse migration vers la Fédiverse et Mastodon? 

J'ai choisi de passer du côté des administrateurs en mettant à disposition un serveur spécialement destiné à la communauté des cartographes, développeurs géospatiaux et autres amateurs de cartes. [Mapstodon.space](https://mapstodon.space) a ouvert ses portes le 5 novembre, porté par un jeu de mots que l'on pouvait difficilement laisser passer, et une série d'émojis tous plus carto les uns que les autres - QGIS, COG, ArcGIS, GDAL, Google Earth ou encore GRASS GIS, tout le monde! 




Choisir son instance
Introduction, profil détaillé
Instance, boost, toot?
Description de l'interface
Suivre des hashtags
Quote RT




[^1]: ?
[^2]: nous communiquons tous par email mais sommes inscrits chez différents fournisseurs de courriel

https://jeffreyfreeman.me/eugen-rochko-ceo-of-mastodon-found-to-support-nazis-agenda/ 

https://ws-dl.blogspot.com/2021/01/2020-01-22-twitter-rewrites-your-urls.html (2020)
https://www.hanselman.com/blog/this-url-shortener-situation-is-officially-out-of-control (2014)


