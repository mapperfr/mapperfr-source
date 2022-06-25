---
title: DocSoc2022
summary: 'Données et métadonnées dans l’hybridation et le bricolage des pratiques des chercheurs en contexte de science ouverte: Un retour d’expérience du GDR SILEX.'
authors: [Christophe Tufféry, Vincent Delvigne, Paul Fernandes, Jérémy Garniaux, Stéphane Renault]
tags: []
categories: []
date: "2019-02-05T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # white, black, league, beige, sky, night, serif, simple, solarized
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
  transition: none
---

### Données et métadonnées dans l’hybridation et le bricolage des pratiques des chercheurs en contexte de science ouverte
Un retour d’expérience du GDR SILEX

![](docsoc_1bandeau.png)

{{< speaker_note >}}

Bonjour à toutes et à tous. Merci aux organisatrices et aux organisateurs pour l'invitation, pour nous donner cette occasion de revenir sur le travail mené au sein du GDR Silex dans la mise en oeuvre d'une plateforme scientifique de cartographie participative, merci enfin pour avoir bien voulu nous accueillir à distance malgré les consignes, suite à des contraintes de dernière minute de notre côté.

{{< /speaker_note >}}


---

#### Équipe

Christophe TUFFERY `(Inrap, TEMPS)`  
Vincent DELVIGNE `(U. de Liège, TEMPS)`  
Paul FERNANDES `(Paléotime, TEMPS)`  
Jérémy GARNIAUX  `(AMU, LAMPEA/MMSH)`  
Stéphane RENAULT `(AMU, LAMPEA)`  

{{< speaker_note >}}
Cette présentation est une contribution collective. proposée par C. Tufféry, VD, PF, SR et moi-même. Je suis le seul non-archéologue de l'équipe puisque je suis géographe, géomaticien et développeur, actuellement en charge du déploiement de la plateforme ArcaDIIS à AMU. Je vais essayer de dire le moins de bêtises possible sur les aspects purement archéologiques de ce travail, et le cas échéant (s'il y en a une qui m'échappe) je vous remercie d'avance pour votre indulgence!
{{< /speaker_note >}}

---

#### Bref historique des recherches

Des travaux menés depuis le XIXe siècle

![](docsoc_hist_rech.png)

{{< speaker_note >}}

Le silex en tant qu'objet scientifique est étudié depuis le XIXe siècle. Déterminer l'origine des silex permet d'appréhender les modes d'exploitation des ressources minérales et la territorialité des groupes humains. Cette figure, extraite de _L'homme primitif_ de Louis Figuier, 1870, est légendée ainsi: "Le premier atelier de l'industrie humaine, ou l'atelier de fabrication et de polissage des silex à Pressigny".

{{< /speaker_note >}}

---

{{< figure src="docsoc_hist_rech_carte1.png" height="100%" >}}

{{< speaker_note >}}
Exemples de cartes produites sur les territoires d'approvisionnement en ressources minérales des préhistoriques
{{< /speaker_note >}}

---

{{< figure src="docsoc_hist_rech_carte2.png" height="100%" >}}

{{< speaker_note >}}
Exemples de cartes produites sur les territoires d'approvisionnement en ressources minérales des préhistoriques
{{< /speaker_note >}}

---

{{< figure src="docsoc_hist_rech_carte3.png" height="100%" >}}

{{< speaker_note >}}
Exemples de cartes produites sur les territoires d'approvisionnement en ressources minérales des préhistoriques
{{< /speaker_note >}}

---

{{< figure src="docsoc_hist_rech_carte4.png" >}} 

{{< speaker_note >}}
Exemples de cartes produites sur les territoires d'approvisionnement en ressources minérales des préhistoriques
{{< /speaker_note >}}

---

{{< figure src="docsoc_hist_rech_carte5.png" >}}

{{< speaker_note >}}
Exemples de cartes produites sur les territoires d'approvisionnement en ressources minérales des préhistoriques
{{< /speaker_note >}}

---

#### Constats

{{% fragment %}} - Diversité des approches {{% /fragment %}}
{{% fragment %}} - Hétérogénéité dans les descriptions {{% /fragment %}}
{{% fragment %}} - Partage difficile {{% /fragment %}}
{{% fragment %}} - Géolocalisation approximative {{% /fragment %}}
{{% fragment %}} - Cartes statiques, _print_ mais pas web {{% /fragment %}}  
{{% fragment %}} - Travaux locaux isolés {{% /fragment %}}  
{{% fragment %}} - Quels schémas explicatifs à petite échelle? {{% /fragment %}}

{{< speaker_note >}}
Une série de constats peut-être faite sur ces premiers travaux:

D'abord, la diversité des approches, méthodes, domaines d'études, etc. crée une grande hétérogénéité dans les descriptions et les caractérisations des matériaux siliceux, d'où découle un certain nombre de difficultés pour partager les données entre chercheurs. 

Ensuite, la géolocalisation de nombreuses données récoltées sur le terrain pose problème car pas toujours bien enregistrée. Les cartes réalisées sont jusqu'ici statiques, peu partageables, plus adaptée à des supports "print", papier ou pdf, qu'à une circulation sur le web. 

Les travaux restent isolés, très localisés, et ne donnent pas lieu à des synthèses multirégionales, ce qui participe à l'impossibilité de proposer des schémas explicatifs valables sur de grands espaces (à petite échelle).

{{< /speaker_note >}}

---

#### Mise en place du GDR 

{{% fragment %}} - Organiser et animer la production de connaissances harmonisées {{% /fragment %}} 
{{% fragment %}} - Mise en place de 4 PCR "Réseau de lithothèques" (2006) {{% /fragment %}} 
{{% fragment %}} - Mise en place du Groupement de Recherche SILEX (2019-2023) {{% /fragment %}} 

{{< speaker_note >}}

Le besoin a donc émergé d'organiser et d'animer la production de connaissances harmonisées sur les formations à silicite qui ont pu être exploitées par les populations préhistoriques.
4 projets collectifs de recherche "Réseau de lithothèques" sont mis en place à partir de 2006 (ARA, CVDL, NA et IDF - d'autres PCR en projets dans d'autres régions).
Le Groupement de Recherche Silex est créé en 2019, avec trois axes de travail:

- Territorialité et mobilité: caractérisation des silex marqueurs
- Des outils harmonisés pour la recherche
- Prospective: réseau international

{{< /speaker_note >}}

---

#### Éléments de méthode

{{% fragment %}} - Inventaire et description harmonisée {{% /fragment %}}
{{% fragment %}} - Méthode harmonisée de caractérisation {{% /fragment %}}
{{% fragment %}} - Pétroarchéologie (interface géologie/archéologie) {{% /fragment %}}

![](docsoc_methode.png)

{{% fragment %}} Paléo-territoires {{% /fragment %}}
{{% fragment %}} -> Litho-espaces {{% /fragment %}}

{{< speaker_note >}}

En termes méthodologiques, il s'agit de mener un inventaire des formations à silicite pour la France et d'en établir une description harmonisée, puis de définir une méthode harmonisée de caractérisation des échantillons présents dans les lithothèques ou prélevés lors de prospection. Ce sont les outils de la pétroarchéologie, discipline à l'interface entre géologie et archéologie, qui sont mobilisés ici.

L'objectif des études est de caractériser le milieu minéral, et de contribuer à la définition des systèmes techno-économiques. Les méthodes d'observation sont complémentaires, et les techniques d'exploration sont multiples.

La finalité scientifique de ces divers outils réside dans la possibilité de reconsidérer la notion de « territoire » en Préhistoire, aujourd’hui marquée par une conception sédentaire et moderne diamétralement opposée à celles des collectifs non-modernes mobiles. La notion de paléo-territoires est actuellement révisée pour la notion de litho-espaces, qui se limite à la description des espaces d'approvisionnement en ressources lithiques. 

{{< /speaker_note >}}

---

#### Données géologiques
##### Des sources hétérogènes

{{< figure src="docsoc_source_donnees.png" resize_options="100x100" >}}

{{< speaker_note >}}

Les données géologiques utilisées sont issues de plusieurs sources: des données de terrain, des cartes et données du BRGM (notamment les webservices d'InfoTerre et la BD-Charm50, les cartes géologiques départementales au 1/50000e fournies au format shapefile sous licence ouverte Etalab 2.0), de la documentation scientifique, etc. 

{{< /speaker_note >}}

---

#### Plateforme cartographique

![](docsoc_carto1.png)

{{< speaker_note >}}
La plateforme cartographique actuelle est constituée d'un ensemble d'outils numériques qui s'appuient sur des normes d'interopérabilité. L'élément central est le serveur cartographique ArcGis Online, auquel viennent se connecter différentes applications clientes: interface carto web, application de saisie mobile, SIG open source QGIS, etc. 
{{< /speaker_note >}}

---

##### ArcGis Online

![](docsoc_carto2.png)

{{< speaker_note >}}
Depuis 2017, le GDR s'appuie sur une application web hébergée par ArcGis Online, développée avec le Web AppBuilder d'ArcGis. Cette interface de webmapping a évolué en fonction des retours utilisateurs, et constitue la première itération d'une interface de partage des données sur les formations à silicite et les points de collecte.

Cette première copie d'écran présente les points de collectes validés pour la France métropolitaine, les Antilles et la Sardaigne.

{{< /speaker_note >}}

---

##### ArcGis Online

![](docsoc_carto3.png)

{{< speaker_note >}}
En se rapprochant, on découvre l'ensemble des points de collectes pour la France et les pays limitrophes, ainsi qu'une couche qui indique l'état d'avancement de l'enquête (les secteurs grisés ne sont pas encore enquêtés)
{{< /speaker_note >}}

---

##### ArcGis Online

![](docsoc_carto4.png)

{{< speaker_note >}}
Cette dernière copie d'écran, centrée sur le Centre Val de Loire, laisse apparaître (en plus des points de collecte) la cartographie des formations à silicite. Cette couche carto est un produit composite, dérivé de la BD-Charm50.
{{< /speaker_note >}}

---

##### Formations à silicite

![](docsoc_carto5.png)

{{< speaker_note >}}
A partir de la base du BRGM, une sélection des formations à silicite est effectuée par des experts. Certaines données attributaires sont supprimées, d'autres ajoutées. 
{{< /speaker_note >}}

---

##### Formations à silicite

![](docsoc_carto6.png)

{{< speaker_note >}}
Les données finales sont publiées en WFS (service web), sous licence ouverte Etalab 2.0 comme l'impose la licence d'origine. Elles sont accessible via QGIS comme services d'entités ArcGIS (serveur ArcGIS REST).
{{< /speaker_note >}}

---

##### Formations à silicite

![](docsoc_carto7.png)

{{< speaker_note >}}
Dans QGIS, elles peuvent être interrogées comme n'importe quelle couche vecteur, et peuvent être enregistrées en local dans divers formats. 
{{< /speaker_note >}}

---

##### Points de collecte et inventaires de lithothèques

![](docsoc_carto8.png)

{{< speaker_note >}}
Les données sur les points de collecte (prospections) et d'inventaire de lithothèques alimentent deux couches de points: les points non validés (en cours) et points validés
{{< /speaker_note >}}

---

##### Points de collecte et inventaires de lithothèques

![](docsoc_formulaire1.png)

{{< speaker_note >}}
Les données proviennent d'un formulaire descriptif harmonisé disponible sous plusieurs formes : fiche papier, fichier tableur, formulaire en ligne, application mobile.
{{< /speaker_note >}}

---

##### Points de collecte et inventaires de lithothèques

![](docsoc_formulaire2.png)

{{< speaker_note >}}
Le formulaire est disponible en ligne (accessible via un navigateur Web) pour les inventaires de lithothèques réalisés en dehors du terrain.
{{< /speaker_note >}}

---

##### Points de collecte et inventaires de lithothèques

![](docsoc_survey123_1.png)

{{< speaker_note >}}
L'application mobile permettant la saisie sur le terrain s'appuie sur ArcGIS Survey123.
{{< /speaker_note >}}

---


#### Migration vers une infra open source

![](docsoc_qwc2_1.png)
Affichage des données QGIS Server dans QWC2

{{< speaker_note >}}

- Nouvelle infra carto: En 2020, l’équipe du projet a décidé de s’engager dans la migration des solutions actuellement mises en œuvre, vers des solutions open source. En parallèle de cette décision, les autres décisions suivantes ont été prises:
  - la publication des données sous licence Etalab 2.0;
  - le dépôt régulier de versions consolidées des données sur la plateforme ArcaDIIS;
  - la mise en ligne de documents iconographiques sur la plateforme Nakala d’HumaNum
  - l’établissement de liens entre les données et ces ressources documentaires.

Ces choix s’inscrivent dans le cadre des orientations des deux plans nationaux pour la science ouverte (2018-2021 et 2021-2024) du MESRI. Une première phase de migration de la solution développée sur les solutions ESRI, a consisté à déployer un serveur cartographique utilisant la solution QGIS Server et une applicative de consultation cartographique s’appuyant sur QWC2, un client Web pour QGIS Server. 

Pour l’instant, le projet QGIS utilise les services de données Web WFS actuellement hébergés sur la plateforme AGOL. Ils seront ensuite importés dans une base PostGIS lorsque nous basculerons complètement sur QGIS et que nous pourrons "débrancher" la solution ESRI.
ESRI.

{{< /speaker_note >}}

---

#### Migration vers une infra open source

![](docsoc_mergin_1.png)

{{< speaker_note >}}

La seconde partie de la migration est prévue pour le deuxième semestre 2022. Une application mobile fournie Mergin Maps, adaptée à la saisie de données sur le terrain et à la synchronisation avec une infrastructure QGIS (fichier projet et synchronisation serveur), viendra remplacer l'application Survey123 d'ArcGIS. Nous avons déjà mené des tests concluants qui nous confortent dans le choix de cette solution. 

{{< /speaker_note >}}

---

 #### Briques de la plateforme à venir

{{% fragment %}} - Dépôts semi-automatisés dans ArcaDIIS {{% /fragment %}}
{{% fragment %}} - Dépôts iconographiques dans Nakala {{% /fragment %}}

![](docsoc_nakala_1.png)


{{< speaker_note >}}

En plus de ces solutions cartographiques open source, d'autres "briques" complètent la plateforme. 

- Des exportations régulières des données seront déposées de façon semi-automatisée sur la plateforme ArcaDIIS (arcadiis.science), qui permettra leur FAIRisation en enrichissant les métadonnées et en leur attribuant un identifiant pérenne. Les données seront accessibles via un moteur de recherche à facettes en interrogeant leurs métadonnées normalisées (Dublin Core ISO 15836, complétée par d'autres normes comme INSPIRE ou le Darwin Core).
ArcaDIIS proposera également la pré-génération de trames de _data papers_ depuis les métadonnées des jeux de données, et - sous la forme d'un Linked Open Vocabulary - l'accès aux mots-clés issus du thésaurus PACTOLS (été 2022).

-Ensuite, les documents iconographiques contiueront à être déposés sur Nakala. Des liens seront établis entre les données et ces ressources documentaires. 

{{< /speaker_note >}}

---

#### De la science ouverte en archéologie

![](docsoc_terrain1.png)

Hybridation des pratiques

{{< speaker_note >}}

Depuis 2006, date du début de nos premiers projets, les notions de science ouverte ont progressivement émergé et se sont de plus en plus diffusées dans nombre de domaines scientifiques. L’archéologie fait partie des disciplines où la traduction dans les faits des principes de l’ouverture des données et des outils n’est pas aussi développée que dans d’autres disciplines, pour différentes raisons - notamment les questions de propriétés des savoirs et des savoir-faire, ou les craintes de pillage des sites archéologiques existant. 

On a pu constater qu'une forme de stratégie d'hybridation des pratiques a été mise en oeuvre par les chercheurs face au mouvement de la science ouverte. Hybridation au sens donné par Latour lorsqu'il décrit les formes d'adhésion et de résistance, de fluidité et de tension dans les relations entre individus et objets matériels - qu'il décrit sous le vocable commun "d'actants". Ici, l'hybridation des pratiques est la dynamique qui amène l'activité scientifique (ou l'enquête de terrain, par exemple) à ne pas se dérouler exactement comme prévu. 

Concrètement, la question des métadonnées est un bon exemple: si l'on sait en théorie que des métadonnées bien renseignées participent au premier plan à une bonne qualité des données et donc au bon respect des principes FAIR, les contributeurs n'en font pas toujours une priorité. Il y a la difficulté à distinguer données et métadonnées, ou bien l'idée que les métadonnées pourront être renseignées "plus tard" parce que ça prend beaucoup de temps pour un intérêt en apparence moindre.

{{< /speaker_note >}}

---

#### De la science ouverte en archéologie

![](docsoc_terrain2.png)

Bricolage cognitif

{{< speaker_note >}}

Cette hybridation produit du "bricolage" cognitif, au sens de la possibilité de s'adapter à un contexte contraint par le caractère limité des moyens dont on dispose. Dans notre cadre de pratiques numériques, les chercheurs s'adpaptent avec leurs compétences et leurs savoir-faire. L'appropriation n'est possible que si ces pratiques peuvent s'intégrer dans des pratiques préexistantes, aussi bien à titre individuel que dans le ou les gorupes dans lesquels ils interviennent et interagissent. 

Pour faire référence à une notion proposée par Marcel Mauss, et en l’adaptant aux dispositifs numériques, la mise en œuvre de ceux-ci ne peut donner
lieu à des « actes traditionnels efficaces » qu’à la condition qu'ils s’inscrivent dans une continuité et non pas dans une recherche de rupture avec les pratiques traditionnelles préexistantes. Pour citer Mauss: « Il n'y a pas de technique et pas de transmission, s'il n'y a pas de tradition ».

En ce sens, on peut considérer que les principes de publication qui soutendent la science ouverte doivent contribuer d’abord à des pratiques de partage, de transmission des savoirs et des savoir-faire dans une éthique de la recherche animée par le respect des autres et donc de la diversité des pratiques de
recherche.

{{< /speaker_note >}}

---

#### De la science ouverte en archéologie

![](docsoc_braconnage.png)

Braconnage culturel

{{< speaker_note >}}

Au sein du GDR Silex, les chercheurs se sont appropriés les pratiques que nous avons mises en place par des processus de « braconnage culturel »: l'expression est de Michel De Certeau et désigne les ruses dont font preuve certains acteurs par des tactiques de résistance, voire de subversion des groupes auxquels ils appartiennent. 

En adoptant lentement les nouvelles pratiques numériques qui leur étaient proposées, et en y résistant « en douceur », de façon presque invisible, certains des membres ont réussi, de l’intérieur même des collectifs de travail, à ne pas se faire imposer ces nouvelles pratiques, comme nous avons pu le constater notamment lors de sessions de formation sur le terrain.

(On voit ici, par exemple, un cas de braconnage: la coexistence de l'utilisation de l'appli mobile et du formulaire papier pour l'enregistrement des données de terrain lors d'une session de formation)

Plusieurs outils et méthodes existent pour accompagner les changements des pratiques: expression des besoins non seulement des changements attendus mais aussi des maintiens nécessaires de l’existant, rédaction collaborative de documents référençant des pratiques « vertueuses », actions de formation, recueil des retours d’expérience, adaptations des protocoles et des dispositifs numériques à la diversité des capacités et des intentions des individus de se les approprier. 

La coexistence au sein d’un même projet de recherche comme le nôtre, de formes d’expression et d’action aussi variées que le changement et la continuité, le souhait de rupture avec le passé des uns, l’envie de conservation de l’existant des autres, permet de souligner certains des paradoxes de la science ouverte et de soulever des questions de nature éthique.

{{< /speaker_note >}}

---


#### De la science ouverte en archéologie

![](docsoc_ethique.png)

{{< speaker_note >}}

Pour clore ce retour d’expérience, nous souhaitions évoquer certaines questions éthiques apparues lors de la mise en œuvre de l’application mobile, en particulier en regard de la publication sous licence ouverte des données produites par les chercheurs sur le terrain.

Parmi les données recueillies, celles concernant les prospections de terrain et les inventaires de lithothèques intègrent des données à caractère personnel dont la géolocalisation des chercheurs ayant saisi les données sur terrain. Or, les acteurs concernés n’ont que rarement conscience des conditions de stockage ou des modalités de diffusion de ces données.

Il nous a semblé que les risques de pillage de lieux patrimoniaux (sites archéologiques ou gîtes de matériaux siliceux), liés à la diffusion des données enregistrées, posait davantage de problèmes que la diffusion des données personnelles des enquêteurs. 

En effet, il est possible de restituer les pratiques de travail d’un chercheur jour par jour (et même heure par heure) à partir des métadonnées non-anonymisées qu’il a produites avec l’application mobile. On peut ainsi visualiser les déplacements par dates et par heures, dans l’ordre où ces données ont été renseignées. Les données et métadonnées sur les relevés de terrain renseignent par conséquent sur les pratiques de travail des chercheurs sur leurs terrains respectifs.

Le fait de voir ces données diffusées sur l’application cartographique n’a soulevé, pour l’instant, aucune question ni refus, alors que dans le même temps, des craintes claires ont été exprimées sur la diffusion des données de localisation des points de collecte - eu égard aux risques de pillage des sites.

Pour la communauté scientifique concernée, la valeur patrimoniale des gîtes semble davantage problématique que la valeur des données à caractère personnel et les risques de leur diffusion.

On peut émettre aussi l’hypothèse que les inconvénients à voir les données à caractère personnel diffusées sont moindres en comparaison des bénéfices tirés de l’usage de l’application mobile. Celle-ci permet enfin aux chercheurs de participer à une œuvre collective de production de données selon un même modèle et un même cadre d’acquisition, ce qui a longtemps été un point majeur de difficultés à la collaboration.

Ces questions sont abordées dans le cadre de la thèse de Christophe Tufféry en cours depuis 2019 à CY Cergy Paris Université en relation avec l’Institut National du Patrimoine (Inp), portant sur les effets du numérique sur l’archéologie et les archéologues. 

{{< /speaker_note >}}

---

#### Merci pour votre attention!

jeremy.garniaux@univ-amu.fr
![](docsoc_1bandeau.png)
