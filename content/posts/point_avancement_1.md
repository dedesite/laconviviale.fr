---
title: "Point d'avancement #1"
date: 2021-09-06T17:55:43+02:00
author: "Andréas Livet"
toc: true
---

Bienvenue dans la première newsletter consacrée à la conviviale, le véhicule électrique, low tech et open source destiné à la campagne et aux autres contrées !

Le projet a démarré depuis peu, mais vous allez voir, il y a beaucoup de choses à dire !

Je tente un format de newsletter assez inhabituel avec beaucoup de contenu technique. Ceux que ça n'intéresse pas pourront se contenter de lire le résumé de chaque section.


## Présentation de l’équipe

Avant tout, il convient de vous présenter les personnes qui travaillent bénévolement sur le projet

* Andréas Livet : initiateur du projet. Développeur et formateur en informatique depuis plus de 10 ans, je me passionne pour la question écologique depuis longtemps et plus particulièrement les questions technologiques avec un regard « décroissant » et très fortement axé low tech (merci Phillipe Biouix). J’ai participé à la création du fond de dotation « Agir Low Tech » et participe modestement à la création d’un superbe tiers lieu à Latillé : Le sens du fil
* Arno : l’homme aux mille idées. Passionné de voiture dans sa jeunesse (BTS en combustion interne), il s’oriente après dans le bâtiment et devient thermicien, puis enseignant en étude des constructions. Ce « touche à tout » revient donc à ses premiers amours avec la conviviale et nous apporte un vrai regard de designer. Il débusque des trouvailles dans les tréfonds d’internet dans ses nuits d’insomnies.
* David : Grand bricoleur devant l’éternel, David a une passion pour les vélos ainsi que pour leur électrification. Il en a fait son activité principale il y a 10 ans et conçoit maintenant ses batteries. Il a installé plus de 200 kits de vélo et conçu autant de batteries. C’est notre référent sur la partie électricité.

## Pourquoi faire une voiture ?

Comme dit Arno, décidément, on a raté un tournant à partir des années 80 dans l’automobile… Et oui, les voitures sont progressivement devenues plus lourdes, sécurisées, confortables, irreparables et bourrées de gadgets inutiles. Malheureusement, la voiture électrique suit cette même pente, alors que les précurseuses, comme la MIA, avaient tout compris !

Il semble qu’aucun constructeur automobile ne souhaite revenir à cette forme de simplicité et délaisse le créneau des véhicules léger (catégorie quadricycle lourds). Il fallait donc que quelqu'un s'atèle à la réalisation de ce fameux « pot de yaourt à roulette » dont parle Biouix !


## Un chassis pour la convi !

{{< rawhtml >}}
<div class="pa2 bg-lightest-blue">
<p><strong>TL;DR</strong> Pour le prototype nous allons prendre un chassis de 4L, car c’était pas cher, répandu et qu’il a la forme idéale (plateforme) pour ce qu’on souhaite faire.</p>
</div>
{{< /rawhtml >}}


La première étape dans la réalisation de notre prototype était de trouver le chassis idéal pour notre projet.
Nous cherchions quelque chose de modulaire, simple et peu coûteux.
Au début, nous nous sommes penché sérieusement sur un des seul châssis open source existant (avec le projet wikispeed) à savoir la [Tabby Evo 4](https://www.openmotors.co/product/tabbyevo/). C’est un projet porté par OpenMotors, société italienne qui conçoit et commercialise une plateforme opensource pour véhicules électriques.

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_a9cefb79ab49689a0ddc1c0b8154f015.png)
*La Tabby Evo 4 places, entièrement Open Source mais finalement peu adaptée au projet*

OpenMotors fournissent en libre acces tous les plans et les modèles 3D du Tabby, mais pas la liste des pièces.

Nous avons finalement décidé de ne pas partir avec pour plusieurs raisons :

- Le prix du chassis nu est excessivement cher pour notre petit budget (~16 000€)
- Si nous voulions le refaire nous même, nous n’avions pas les références des pièces utilisées et OpenMotors n’ont jamais répondu à nos questions. Et oui, car pour que le chassis soit fonctionnel, il faut trouver les bonnes suspensions, le bon moteur, le bon variateur, la bonne direction etc. Autant d’inconnues qui auraient rendues le projet difficilement réalisable en peu de temps.
- Enfin, le châssis est celui d’une petite citadine 4 places avec un rétrécissement à l’arrière et une barre au niveau des suspensions, ce qui contraignait beaucoup le design du véhicule et nous empêchait de faire un utilitaire.

Nous étions alors à la recherche d’un chassis existant, peu onéreux et, si possible, de type plateforme (maintenant on parle de type « skate » pour les véhicule électrique).

On a d’abord cherché dans les véhicules léger des année 80 : C15, AX etc. mais tous ont un chassis monocoque. Très bien pour réduire le poids, augmenté la résistance, mais moins bien quand on veut avoir la liberté de faire ce qu’on veut dans l’habitacle.

On a alors trouvé notre bonheur dans des chassis de conception plus ancienne à savoir ceux de la 4L car : 
- Ces châssis sont de nouveau fabriqué par des équipementier et on trouve des pièces neuves pour tous les éléments (cardans, amortisseurs etc.). Cela pourra être une bonne base pour le véhicule final.
- Enormément de personnes (principalement des jeunes ingénieurs par le biais du 4L trophy) réparent ces voitures et partage leur expérience détaillée en vidéo sur Youtube. J’ai rarement vu une voiture bricoler et retaper par un nombre aussi important de personne.
- C’est une voiture qui correspond à ce que l’on souhaite faire en terme de poids, puissance et dimensions
- Avec la 2CV, elle représente une sorte d’« age d’or » de l’automobile low tech, légère, sans chichi, réparable, tout en étant esthétique.

Début juin, Andréas est donc parti, sur un coup de tête, en covoiturage à Nantes acheter un 4 GTL a une famille qui l’utilisait pour emmener les enfants à l’école. Maintenant grand ados, ils ont vu partir leur 4L avec beaucoup d’émotion. Merci à Grégory !

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_04c642dd3b87236b6ab639622390d4d5.JPG)
*La 4L de retour de Nantes*


N’ayant pas à notre disposition les outils nécessaires pour démonter un moteur, Andréas a posté une annonce leboncoin en proposant de donner les pièces du moteur thermique et de la carrosserie, si la personne venait la démonter. 5 minute plus tard, il recevait un appel de Léopold, ingénieur en électronique (travaillant à Iso Delta, équipementier automobile proche de chez nous) et passionné en véhicules anciens. Il a très vite proposé d’échanger la 4L « fonctionnelle » contre un chassis de 4L dont le moteur était défectueux et de l’aide sur le projet.

Son expertise autant en électronique qu’en véhicules anciens vont être d’une aide précieuse pour la réalisation du prototype.

Et voici le résultat :

Bon c'est un peu rouillé, mais avec un peu d'huile de coude et quelques pièces changées, ça pourrait ressembler à ça :
![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_6f0a79d9ab6a89ebdb6be74ad9bfe2a3.png)


Nous nous occuperons du chassis une fois que toute la partie motorisation et les batteries seront fonctionnelles.

## Un moteur pour la convi !

{{< rawhtml >}}
<div class="pa2 bg-lightest-blue">
<p><strong>TL;DR</strong> Pour le prototype nous avons choisis le moteur de la Renault Twizy, il correspond à nos besoins, se trouve d’occasion et son variateur est bien connu. De plus, d’autres projet de retrofit 4L l’ont utilisé.
</div>
{{< /rawhtml >}}

En parlant du moteur, ça a été aussi toute une histoire !

Nous avons beaucoup échanger à ce sujet : moteurs dans les roues ou central ? Traction ou propulsion ? A courant continu ou alternatif ? Garde-t-on la boite de vitesse ou pas ?

Il a finalement été décidé de partir sur ce qui se fait de plus courant en rétrofit (conversion d'un véhicule thermique en électrique), à savoir d’installer le moteur électrique à la place du moteur thermique en gardant la boite de vitesse d’origine ainsi que les cardans.

C’est par exemple ce qu’on fait Renault Classic et Melun Retro Passion sur leur magnifique retrofit de 4L e-plein Air :

![Photo de la e Plein air](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_a5e2796f6919bb59998c450734607629.png)

Nous avons choisi d’utiliser, comme pour la e-plein air, le moteur de la Renault Twizy pour plusieurs raisons :
- C’est un des rares moteurs disponible sur le marché (aussi bien en neuf que d’occasion) correspondant à cette catégorie de véhicule (L7). On est ainsi sûr qu’en terme de poids et de puissance, ça sera suffisant, sans être sur dimensionné
- La twizy est sans doute le seul véhicule de cette catégorie a avoir été fabriqué en relativement grande série et conçu par Renault. C’est un gage de bonne conception et de qualité.
- Son variateur/onduleur (c’est la partie qui fait le lien entre la batterie, l’accelerateur et le moteur), le SEVCON GEN 4 est bien connue et certains professionnels proposent ce variateur programmé pour le moteur de la Twizy, mais sans les restrictions installées par Renault (voir plus bas)


## J'ai changé mon variateur et elle dépote ma mobilette

Oui, ce terme me rappelle mes années collège où je bricolais ma "brêle".
Sur une mobilette, c'est un élément mécanique qui permet de remplacer une boîte de vitesse.

Dans une voiture électrique, c'est un élément électronique important responsable de plusieurs choses :
- Faire varier l'intensité électrique envoyée au moteur en fonction de l'acceleration
- Dans le cas d'un moteur en courant alternatif, il fait aussi office d'onduleur pour convertir le courant continu des batteries en courant alternatif (triphasé dans notre cas) permettant de faire tourner le moteur
- Gérer le faisceau électrique du véhicule et renvoyer des informations (intensité instantanée, vitesse etc.) via ce qu'on appelle un bus CAN et pouvoir les afficher par la suite sur le tableau de bord par exemple.

Comme dit plus haut, nous avons opté pour le même modèle de variateur que celui de la Twizzy, mais avec une programmation beaucoup plus simple. Il est dans un mode presque "analogique" qui nous permettra en théorie de brancher simplement l'accélerateur, la batterie (via le BMS) et le moteur sans contraintes.

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_2d8061c0c465fd94d2f4601bef2d2cc2.png)
*Le SEVCOM GEN 4 produit en Slovénie*


Nous avons fait appel aux services de [kit elec shop](https://www.kit-elec-shop.com/fr/) (basé à Tours) pour nous fournir un SEVCOM pré configuré et sans doute nous aider par la suite dans nos développements (ajout de fonctionnalités).


Nous tenons à remercier l’équipe de Kit Elec Shop pour leur écoute et leur souplesse.


Nous avons reçu fin août ce magnifique [kit](https://www.kit-elec-shop.com/fr/kits-avec-moteur-asynchrone/4963-kit-electrification-vehicule-48v-sans-moteur-asynchrone-12kw-et-reducteur-sans-batterie.html) que nous avons hâte d'installer.

Cerise sur le gateau : si j'ai bien compris, certains éléments de la configuration du variateur font partie d'un projet [Open Source de Renault](https://www.openmotors.co/renaultpomsignup/) (à l'origine du projet Tabby d'ailleurs). Une bonne base pour un début de matériel ouvert ? Nous verrons bien.

## Et les batteries ?

{{< rawhtml >}}
<div class="pa2 bg-lightest-blue">
<p><strong>TL;DR</strong> Nous allons surement assembler nos propres batteries à partir de cellules cylindre LiFePo3. Le choix du BMS n’est pas encore acté.
</div>
{{< /rawhtml >}}

Vous l’aurez compris, notre spécialiste batteries dans l’équipe c’est David.
Même s’il a beaucoup d’expérience sur l’assemblage de batteries de vélo, une batterie pour voiture électrique est sensiblement différente en terme de dimensionnement.
Pour vous donner une idée, nous souhaitons intégrer à notre prototype une batterie de **6kWh** (comme la Twizy), ce qui représente l’équivalent de **12 batteries de vélo électriques** (500Wh en moyenne).
La puissance délivrée par notre moteur est quand à elle **48 fois plus importante** que celle d’un vélo électrique (12kW contre 250W) ! A comparaison une Tesla à un moteur de plus de **240kW** et embarque minimum **57kWh** de batteries !
A ce compte là on est presque plus proche d'un vélo électrique que d'une Tesla :D.

Il faut donc des cables plus gros (on est sur du courant continu, ça chauffe!) et, dans le cas du Lithium, un BMS de qualité (voir plus loin).
Si le dimensionnement et la chimie de la batterie sont choisis, nous ne sommes pas arrêtés sur le format de cellules : prismatiques, cylindriques de différentes tailles (18650/ 32650 etc)... Le rapport qualité/prix ainsi que l'intégration sur le châssis du prototype vont orienter cette décision.

Pour le prototype, il y a de grande chance pour que ce soit des celulles cylindriques de type 32650 :
![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_c6a334e1eff3f3b77a4462d319487e99.png)
*Le format cylindrique donne plus de liberté dans la forme des batteries*

Pourquoi un tel choix ?
- C’est le meilleur rapport qualité/prix
- David à l’habitude et le matériel pour assembler ces batteries
- Les cellules cylindriques étant plus petites (mais plus nombreuses), elles offrent une souplesse en terme d’aménagement. Dans notre cas, nous souhaitons mettre les batteries à l’intérieur du châssis afin de dégager un maximum de place sur le plateau.

Note : Il se peut aussi que nous partions sur des éléments d'occasion de batteries d'autres voitures afin de réduire les coûts du prototype et perdre moins de temps en conception dans un premier temps. A voir, si nous trouvons des éléments qui nous conviennent.

Côté technologie, nous partons sur du [Lithium Fer Phosphate](https://fr.wikipedia.org/wiki/Accumulateur_lithium-fer-phosphate) pour plusieurs raisons :
- C’est la technologie la plus fiable (non inflammable)
- Elle offre un nombre de cycle plus élevé (entre 1500 et 5000) que les batteries à technologie Cobalt-Nickel (présente dans les Tesla), ce qui laisse espérer une durée de vie possible de 10~15 ans ou 300 000 km !
- Elle ne contiennent pas de Cobalt, élément rare qui fait l’objet de beaucoup de pression et dont l’extraction est très problématique. Les mines sont principalement au congo, « emploient » souvent des enfants et financent des guérillas.
- Elles ont certes une moins bonne densité énergétique (rapport poids/puissance), mais comme on en met peut et qu’on vise une autonomie limitée c’est moins un problème.

Pour l’instant, le choix du BMS (si vous ne savez pas ce que c'est, on en parlerai dans un autre billet soyez rassuré) n’est pas encore arrêté. Idéalement, nous aimerions avoir un matériel open source et open hardware, mais pour le proto, on prendra ce qu’il y a de plus pratique pour nous (technologie connue) et de moins cher sans doute.

## Et à quoi elle va ressembler votre « conviviale » ?

Il se peut qu’elle puisse ressembler à quelque chose comme ça :)

En version léger, les cheveux au vent, that 70's Show, arceaux et bâche (style Méhari), le Honda Vamos 1973

Vidéo de présentation (à imaginer avec un moteur électrique ... moins bruyant)
https://youtu.be/_G_aVo0LtdQ

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_23c30b23dc025694a46e089391b24412.png)

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_4ea363e11c2bbf75bac72e99edf37882.png)
*Pas trop fan du côté militaire mais ça donne une bonne idée de ce qu'on souhaite faire*


https://www.cgtrader.com/3d-models/car/antique/fiat-600-multipla-coriasco-familiare-1956

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_e6f7dd9d397f64b4dd0da4d33af34c23.png)
*En version plus confort et style retro, une modification du carrossier Coriasco sur base fiat 600 multipla de 1956*


Rien d’arrêté pour l’instant mais des grandes lignes structurelles se dessinent :
- Siège conducteur au niveau des roues avant pour gagner un max de place à l’arrière
- 4 sièges très légers pliables, escamotables et plaçables à plusieurs endroits pour une modularité poussée à l’extrême (exemple une ligne de 3 sièges sur le côté gauche du véhicule et toute une longeur disponible pour mettre du matériel).
- Une structure tubulaire simple et plane pour simplifier la réalisation

{{< rawhtml >}}
<iframe width="560" height="315" src="https://www.youtube.com/embed/HgetuwbVLms" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
{{< /rawhtml >}}

C’est Arno le pro du domaine de l’habitacle, il déniche des vieilles voitures méconnues (des protos non commercialisés aussi) mais tellement bien conçues. Nos principales inspirations viennent des voitures des années 60~70 et des keicar (catégorie de petites voitures similaire à nos quadricycles lourds) japonaises.
En voici un petit panorama :

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_a10ed31e76a069a20efe93c1e17cfe3f.png)
*Le XBUS du constructeur Allemand Electricband est un des seul véhicule contemporain à avoir des caractéristiques similaires à ce qu'on souhaite faire.*

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_d72d08ed256d4db5423e328ec500bfa7.png)
*La petite française pixel qui n'a jamais été produite en grande série*

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_82d464a788b2a5f036457e39b42121de.png)


![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_7a0bc0ab2fc4e5a152c674a0f066c7d9.png)
*Un étonnant concept car Honda qui date de plus de 20 ans*


## Un modèle économique différent

{{< rawhtml >}}
<div class="pa2 bg-lightest-blue">
<p><strong>TL;DR</strong>Les clients monteront eux même la voiture dans des ateliers en suivant une formation. Ils ne paieront pas pour un objet fini, mais pour des pièces et une formation. Notre structure sera à but non lucratif.
</div>
{{< /rawhtml >}}

Nous ne comptons pas fabriquer des voitures comme un constructeur classique.
En effet, il nous serait impossible d’être concurrentiel en terme de prix et notre voiture ne serait accessible qu’aux plus riches. Or, nous comptons proposer un prix de vente de 10 000€ (ça sera sans doute un peu plus).
L’objectif est de monter une structure à **but non lucratif** (association ou coopérative) qui s’occupera de l’achat des pièces et de la location des atliers, puis formera les acheteur de la voiture à l’assembler (et donc la réparer eux-mêmes). Les clients, n’acheteront donc pas une voiture, mais des pièces et une formation.
Le but étant de **favoriser l’autonomie** et **réduire les coûts de production** afin de garantir un prix d’achat minimum tout en ayant des pièces (notamment batteries et moteur) de **qualité**.
Le fait de laisser le client faire la dernière étape de l’assemblage, permet aussi de personnaliser son véhicule et de le rendre encore plus adapté à son futur usage (ex : modèle pickup, ajout d’un onduleur 220V pour utiliser les batteries comme un générateur électrique, aménagement minivan etc.)
Nous comptons même aller plus loin en proposant aux clients de venir avec d’assembler la voiture en partie avec des pièces d’occasion (forcément compatibles) prises sur des véhicules anciens.
Pas sûr que ce dernier aspect soit validé par l’UTAC CERAM (laboratoire responsable de l’homologation), mais on va quand même demander ;).


## Et la suite ?
La prochaine étape consistera à réaliser une pièce de jonction entre la boite de vitesse et le moteur de la twizy, à l’instar de ce qu’a fait [ce slovène sur un rétrofit 4L](https://www.youtube.com/watch?v=c1RCV6uzLZA).

Pour cela, un habitant de Latillé et bénévole du sens du fil, Bruno, est prêt à nous aider. Il est ancien soudeur pour la division prototype de chez Heuliez (constructeur de la Mia notamment).

Pour la réalisation de la pièce, nous comptons faire appel à un tourneur fraiseur spécialisé dans les voitures anciennes. Andréas leur emmène le moteur et la boîte la semaine prochaine.


## Quand pourra-t-on rouler en « convi » ?

Très bonne question ! La réponse dépend principalement de l’engouement que succitera le projet auprès du public et des institutions.

Voici les différentes étapes envisagées avec un angle optimiste :
    • Jusqu’à fin 2021 : réalisation d’un premier prototype qui servira d’illustration du concept en terme d’usage et d’habitacle. Il ne sera pas homologué et sera sans doute assez éloigné du produit final en terme de technologie (chassis, moteur, batteries, carroserie)
    • 2022 : Campagne de financement participatif en vue de réaliser un véhicule de pré-série qui servira de base à l’homologation (min 60 000€ !). Là seront fait les choix définitifs en termes de pièces et technologie fournisseur.
    • A partir de 2023 minimum : début des premiers ateliers de formation/montage et 1ère conviviales sur les routes de France et pourquoi pas d’Europe ?

## Futurs partenaires

L'autre jour, Andréas a pris contact avec Frédéric Mourier, Designer industriel et fondateur du [projet Avatar](https://avatar-project.fr).

Malgré un design très différent, nos projets sont très similaires dans leur approche et leur objectif.

Nous envisageons une collaboration à grande échelle avec différents acteurs de la mobilité "alternative". Vous aurez sans doute plus d'informations dans la prochaine newsletter.

![](https://s3.standard.indie.host/pad-lamyne-org/uploads/upload_4e5a71b15bf02ca9843e06351d12e43d.png)
*Très futuriste, le projet Avatar ambitionne de faire un véhicule consommant 3 à 5 fois moins qu'une voiture électrique "classique"*

## Le mot de la fin

Merci d'avoir pris le temps de lire cette newsletter jusqu'au bout.

Nous espérons vous présentez la prochaine fois le chassis avec le moteur de la Twizy monté dessus !

Comme on dit : « la route est longue, mais la voie est libre ! »