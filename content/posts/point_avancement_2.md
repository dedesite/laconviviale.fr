---
title: "Point d'avancement #2"
date: 2022-02-23T17:55:43+02:00
author: "Andréas Livet"
toc: true
---

Cela fait bien longtemps que je n'avais pas donné de nouvelles du projet, il était donc temps de vous tenir informé des derniers avancements.

## La conviviale intègre le tiers lieu "Le sens du fil"

Vous vous rappelez sans doute que je bricolais le chassis de la 4L dans mon jardin. Bien évidement cela avait des limites et il fallait à la conviviale un toit au dessus de la tête ainsi qu'une structure juridique à laquelle elle serait adossée pour pouvoir éventuellement faire des demandes de subvention et répondre à des appels à projet.

Participant depuis quelques années à la création d'un tiers lieu dans notre village (Latillé, 86) il était tout naturel que la conviviale rejoigne ce projet qui abrite déjà un atelier bois partagé, une recyclerie et bientôt un café associatif. Ce lieu a pour vocation de soutenir les intiatives locales autour des problématique de transition écologique.

La conviviale va avoir un espace dédié où l'on pourra effectuer les tests, répartions et autres assemblages.
Cet espace servira aussi de vitrine pour le projet et je l'espère donnera envie à d'autres de participer à l'aventure !

Vous pouvez me voir ici lors de notre AG, présentant les différentes pièces constituant le futur véhicule.

![](/img/sens_du_fil.jpg)

## Etat du chassis

J'ai entièrement démonté le chassis de la 4L dans le but de le restaurer.

J'ai l'ai entièrement poncé et malheureusement, il est en moins bon état que prévu : il y a des larges trous de rouille dans les longerons et à d'autres endroits, de plus il va falloir refaire le circuit de freinage que je n'ai pas pu démonter sans l'abimer.

Rien d'insurmontable, des pièces de rechange sont disponibles sur internet, mais ça rajoute une étape et des dépenses non prévues.

Dès que la température le permettra (il fait bien froid au sens du fil), les travaux de restauration reprendront.


## Batterie : le choix du pragmatisme

Grâce aux généreux financements de proches (merci Ben, Aurel et Mathias), nous avons pu acheter les différents composants nécessaires à l'électrification de la 4L.

Par pragmatisme, nous avons décidé d'acheter un bloc batterie déjà éprouvé à savoir [un pack de batterie de la VolksWagen ID.3](https://evshop.fr/en/home/339-vw-id3-battery-module-5940092366347.html). Elle fait partie des batteries avec la densité énergétique la plus importante et son caisson en aluminium est resistant et ses dimension sont parfaites (surtout la hauteur : 11 cm). Il logera sans problème dans le chassis de la 4L. Evitant ainsi que prendre de la place ailleurs.

En revanche, question chimie, ce n'est pas du Lithium Fer Phosphate comme nous aurions souhaité, mais du Lithium-Manganèse-Cobalt. Il s'agit de [celulles produite par LG Pologne](https://cleantechnica.com/2020/06/11/lg-chem-began-mass-production-of-ncm712-batteries-in-poland-in-q1/), ce sont les mêmes que dans la Renault Zoé.

Donc, de ce côté là rien de bien écologique, si ce n'est le fait qu'au lieu d'embarquer minimum 7 pack de batteries (soit 230kg pour 45kWh) [comme l'ID.3](https://en.wikipedia.org/wiki/Volkswagen_ID.3), nous n'en embarquons qu'un seul (soit 33kg pour 6,85kWh).
De plus, ce sont des packs d'occasions, parfait pour la réalisation de notre prototype.

Bien sûr, vous le savez déjà, avec une si "petite" batterie, la conviviale n'aura pas l'autonomie des voitures électriques actuelles. Si l'on prend l'autonomie annoncée d'une ID.3, on tombe à 50km pour 1 pack de batterie, espérons qu'en étant plus légère et moins puissante, la conviviale puisse faire un peu mieux. C'est un choix assumé, nous voulons concevoir un véhicule qui induit des contraintes à son utilisation et ainsi questionne notre mobilité. La tendance actuelle de développement des véhicules électriques est absolument folle.
Les constructeurs et les politiciens cherchent à nous faire croire que l'on pourra à la fois : remplacer le parc de véhicule thermique par des voitures électriques ayant les mêmes caractéristiques poids/puissance/autonomie, que l'on pourra charger en moins de 30min (je vous dis pas la puissance qu'il faut pour cela) et qu'en même temps on va sortir du nucléaire grâce au développement des énergies renouvellables !
C'est absolument irréalisable et il s'agit clairement d'un mirroir aux alouettes agité à des fins commerciales et électorales...

Nous faisons le choix d'une certaine forme de réalisme et assumons que d'ici quelques années (ou quelques dizaines) la mobilité sera forcément différente. Non pas par choix, mais par contraintes physiques.

Nous gardons comme objectif le fait de pouvoir utiliser des cellules LFP, mais nous n'avons pas trouvé de pack dont les dimensions permettraient de stocker la batterie dans le chassis (qui a une hauteur d'environ 15cm). 
Nous avions envisager de concenvoir notre propre pack de batteries à partir de cellules cylindriques, mais il s'avère que pour de grandes capacités c'est un défis techniques important surtout que c'est pour de la mobilité.
Il y a donc des problèmes d'étanchéité, de fixation, de dimensionnement des cables etc. qui se rajoutent.

Je garde en tête l'idée de pouvoir développer des packs de batteries facilement réparables et "standard", mais ça sera pour une prochaine phase du projet. Pourquoi pas par exemple avoir 6 petits pack de 1kWh de la taille de ceux qu'on peut trouver sur un vélo électrique ? C'est peut-être une piste à creuser, ou à éviter :D.


## Bienvenue au tinyBMS

J'avais rapidement mentionné la problématique du BMS (Battery Management System) dans la newsletter précédente.
C'est un élément crucial dès que l'on utilise des batteries au lithium. En effet, celles-ci peuvent parfois surchaffer ou être en surtension, il faut donc un mécanisme qui permet de couper le courant en cas de problème.
C'est le rôle du BMS. Il protège aussi la batterie de décharges trop profondes.

Les chinois fabriquent toutes sortes de BMS et nous comptions partir sur [ce genre de modèle au début](https://fr.aliexpress.com/item/4000965709746.html) :

![daly-bms](https://ae01.alicdn.com/kf/H6b847ffa8bc14923bb6d4c8858a9dfa53/Daly-BMS-bluetooth-APP-4S-LiFePo4-12V-24V-48V-40A-60A-100A-120A-150A-200A-300A.jpg_640x640.jpg)
*Un exemple de BMS chinois rutilent avec plein d'accessoires mais quid de la fabrication et du support client ? Sans parler des problèmes de livraison et de frais de douanes.*

Le soucis c'est que ce sont des BMS dit "traversant", c'est à dire que le courant provenant de la batteria passe dedans pour aller vers le variateur. Ce n'est pas un gros problème sur des courants de faible intensité, mais avec un moteur de 12kW et 48V, on peut attendre une intensité de 250A, ce qui commence à faire beaucoup !

Ces modèles sont donc ventilés et il y a un risque non négligeable de surchauffe.

Plusieurs spécialistes m'ont donc conseillé de prendre un BMS non traversant qui utilise [un capteur à effet Hall](https://fr.wikipedia.org/wiki/Capteur_%C3%A0_effet_Hall) pour mesurer le courant qui passe dans le fil.

Thierry Lequeu du site [kit elec shop](https://www.kit-elec-shop.com/fr/) m'a parlé d'un BMS intéressant fabriqué en Lituanie : le [tinyBMS](https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36).

![tiny-bms](https://www.energusps.com/website/image/product.template/36_beaad6c/image)
*Il est vraiment petit ce tinyBMS*


Et c'est celui que nous avons choisis pour notre prototype.
Pour plusieurs raisons :
- Nous avons un contact direct avec le producteur, c'est très pratique pour avoir des informations sur la mise en oeuvre par exemple (j'ai déjà posé plusieurs question à leur service client)
- Il est produit en UE
- Pas trop cher
- Dont le courant ne passe pas dans le circuit (avec [un capteur effet HAL](https://www.energusps.com/shop/product/lem-current-sensor-75a-750a-31))
- Modulaire (le port CAN et le bluetooth sont sans doute nécessaire pour le prototype, mais peut-être pas pour la suite)
- Il ne prend pas de place et pourra s'insérer aisément où l'on veut.

Son seul inconvénient : il ne peut pas gérer plus de 16 séries de cellules, ce qui limite le nombre de batteries que nous pourrons utiliser. Notre pack de batteries actuelle contient vraissemblablement 12 ce qui sera suffisant.

Nous avons hâte de pouvoir commencer les essais, espérons que tout fonctionne bien !

## La pièce introuvable

Techniquement, la conviviale est ce que l'on appelle un "[retrofit](https://fr.wikipedia.org/wiki/R%C3%A9novation_(ing%C3%A9nierie)#Conversion_d'un_v%C3%A9hicule_thermique_en_v%C3%A9hicule_%C3%A9lectrique)", c'est à dire l'électrification d'un véhicule thermique. Plusieurs entreprises se sont spécialisées dans ce domaine, avec notamment la conversion de véhicule récent comme les [renault clio](https://transition-one.fr/produit/retrofit-clio-3/), mais aussi de véhicules plus anciens comme [les 2CV et les Mehari](https://www.mehariclub.com/fr/r-fit/).

Plusieurs rétrofit de 4L ont aussi été réalisés (j'avais évoqué la 4L ePlein Air dans le précédent billet), mais toujours des pièces uniques à ma connaissance.

La difficulté de ce genre de travaux est de pouvoir insérer dans un chassis ancien des pièces modernes ayant une mécanique bien différente.

Cela peut-être pour trouver un bon emplacement pour les batteries par exemple, ou bien, dans notre cas, de pouvoir assembler le moteur de la Twizy avec la boite de vitesse de la 4L.

Pourquoi avons-nous besoin de la boite de vitesse de la 4L me direz-vous ? Et bien, parcequ'une boite de vitesse contient plusieurs mécanismes essentiels au bon fonctionnement d'une voiture qui sont :
- le lien avec les [cardans](https://fr.wikipedia.org/wiki/Joint_de_Cardan). Ce sont eux qui permettent de transmettre la force motrice du moteur vers les roues. Et oui, comment les roues de votre voiture peuvent toutes les deux tourner et avec un angle de braquage alors que le moteur est fixe ? Grâce aux cardans. Toutes les voitures en possède et dans le cas des retrofit, il est souvent beaucoup plus simple de garder les cardans d'origine que de tenter d'adapter les cardans spécifiques au véhcule électrique d'origine (dans notre cas la Twizy) sur l'ancien chassis (plus de détail la dessus plus bas).
- le [différentiel](https://fr.wikipedia.org/wiki/Diff%C3%A9rentiel_(m%C3%A9canique)) qui permet au roue de en pas tourner à la même vitesse dans les virages. C'est essentiel pour la tenue de route et là encore, toutes les voitures ont un système de différentiel plus ou moins poussé
- un mécanisme de réducteur du nombre de tour moteur (qui est de l'ordre de 3000 trs/min sur une essence), vers les roues. Sur une voiture thermique, cela passe par la boite de vitesse et l'embrayage qui permet de changer les rapport et ainsi de pouvoir mieux utiliser la puissance du moteur thermique dont le couple n'est pas le même à bas régime. Sur un moteur électrique, le couple est quasiment pareil sur toute la plage d'utilisation du moteur, ce qui rend la nécessité de changer de vitesse caduque. En revanche, il y a toujours besoin d'un réducteur et la boite de vitesse de la 4L positionnée en troisième vitesse fera très bien l'affaire. Vu qu'on ne souhaite pas dépasser les 80km/h, ça sera idéal.

Autre raison pour garder la boite de vitesse et ne pas utiliser le [réducteur de la twizy](https://www.kit-elec-shop.com/fr/kits-avec-moteur-asynchrone/4962-moteur-asynchrone-12kw-et-reducteur-differentiel-renault-twizy.html) : la boite de la 4L est dans l'axe du moteur, ce qui fait que l'on a pas besoin de modifier le chassis pour l'assemblage. Il faut simplement fabriquer un support moteur à la place du moteur thermique (il y a déjà des point d'accroche prévu pour cela) et positionner le moteur électrique dans l'axe (voir photo).

Si l'on voulait prendre le réducteur de la twizy, ça serait une toute autre affaire. En effet, il n'est pas dans l'axe du moteur. Il faudrait donc faire des modification importantes sur le chassis pour pouvoir fixer et positionner le réducteur. Mixer les cardans de la twizy à ceux de la 4L et enfin, positionner le moteur de la twizy en travers du chassis et non aligné, comme c'est le cas du moteur initial (voir photo).

![moteur-reducteur-twizy](https://www.kit-elec-shop.com/23389-large_default/moteur-asynchrone-12kw-et-reducteur-differentiel-renault-twizy.jpg)
*Le moteur est en travers du réducteur*

Donc, maintenant que l'on sait que l'on a besoin de la boite de vitesse originale, comment fait-on pour que le moteur électrique puisse transmettre sa puissance à la boite ?

C'est un problème en apparence relativement facile : le moteur à une "prise de force" qui acceuile un axe cranté et la boite de vitesse a justement un axe cranté.
Le souci c'est qu'il n'ont pas les mêmes diamètre, ni le même nombre de crans.
De plus, la boite et le moteur n'ont pas du tout la même forme. Pour résourdre ce problème, il faut fabriquer ce que l'on appelle une platine qui permettra de faire la jonction entre les deux.
C'est un travail de tourneur fraisage relativement facile à ce que j'en ai compris.

Pour l'accomplement du moteur et de la boite, c'est une autre affaire. Généralement, les tourneurs fraiseurs utilisent ce que l'on appelle des pièces d'accouplement (voir photo). C'est un mécanisme assez standard composé généralement de 2 pièces qui vont s'emboiter dans chacune des parties et se relier pour transmettre la forme rotative du moteur à l'autre extrémitée.

![piece-accouplement](https://www.hydrodis.com/1143/flector-d-accouplement.jpg)
*Exemple de pièce d'accouplement dit "elastique"*

Malheureusement, la prise de force de la boîte de vitesse, n'est pas standard et, selon les tourneurs fraiseurs à qui j'ai fais appel, il n'est pas aisé de fabriquer une pièce d'accouplement qui s'adapterai à la boite de la 4L.

Une piste serait d'utiliser le volant moteur présent sur l'embrayage sur lequel on pourrait plus aisément fixer une pièce standard. C'est par exemple ce qu'a fait [ce Slovène (dont j'ai déjà parlé sur sa 4L](https://www.youtube.com/watch?v=c1RCV6uzLZA).

Les tourneurs fraiseurs à qui j'ai fais appel, on finalement jeter l'éponge : ils avaient trop de boulot avec d'autres clients et bien qu'ils aiment ce genre de défis, ce n'est pas avec ça qu'ils gagnent de l'argent, c'est trop spécifique.

J'ai alors contacter le fournisseur de pièce pour voiture de collection [Melun Retro Passion](https://www.melun-retro-passion.com/fr) qui est à l'origine de la 4L ePlein Air pour avoir le contact du tourneur fraiseur qui leur a réaliser la pièce, mais ce dernier ne souhaite pas fournir ses plans. J'attend les coordonnées d'une autre entreprise capable de ce genre de chose, mais rien est sûr.

J'ai quelques autres pistes et vais tâcher de les explorer ces prochains jours, je vous tiendrai au courant.

Quoiqu'il en soit, cette pièce est essentiel au projet, sans elle, nous ne pouvons même pas faire des essais moteur sur table, car le moteur de la twizy n'a qu'un seul roulement et à besoin d'être fixé à son réducteur pour tourner sans s'abîmer.
Le travail sur l'aspect mécanique est donc à l'arrêt tant que nous n'avons pas cette pièce.

A moins, d'acheter un réducteur de twizy et faire les essais avec, puis le revendre au moment d'avoir la pièce. Mais ce sont des pièces relativement chères et je ne sais pas si ça se revend bien. Ce n'est pas tout le monde qui a ce genre de besoins...

## La suite

Vous vous en doutez, nous allons continuer à travailler sur la restauration du chassis et arriver à trouver une solution pour la pièce d'accouplement.

Aussi, vous aurez sans doute bientôt des images de l'habitacle, je n'en dis pas plus... :)

A bientôt !