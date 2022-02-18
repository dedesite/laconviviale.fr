---
title: "Point d'avancement #2"
date: 2021-09-06T17:55:43+02:00
author: "Andréas Livet"
toc: true
---

Cela fait bien longtemps que je n'avais pas donné de nouvelles du projet, il était donc temps de vous tenir informé des derniers avancements.

## La conviviale intègre le tiers lieu "Le sens du fil"

Vous vous rappelez sans doute que je bricolais le chassis de la 4L dans mon jardin. Bien évidement cela avait des limites et il fallait à la conviviale un toit au dessus de la tête ainsi qu'une structure juridique à laquelle elle serait adossée pour pouvoir éventuellement faire des demandes de subvention et répondre à des appels à projet.

Participant depuis quelques années à la création d'un tiers lieu dans notre village (Latillé, 86) il était tout naturel que la conviviale rejoigne ce projet qui abrite déjà un atelier bois partagé, une recyclerie et bientôt un café associatif. Ce lieu a pour vocation de soutenir les intiatives locales autour des problématique de transition écologique.

Vous pouvez me voir ici lors de notre AG, présentant les différentes pièces constituant le futur véhicule.

TODO : insérer la photo

## Etat du chassis

J'ai entièrement démonté le chassis de la 4L dans le but de le restaurer. 
J'ai l'ai entièrement poncé et malheureusement, il est en moins bon état que prévu : il y a des larges trous de rouille dans les longerons et à d'autres endroits, de plus il va falloir refaire le circuit de freinage que je n'ai pas pu démonter sans l'abimer.

Rien d'insurmontable, des pièces de rechange sont disponibles sur internet, mais ça rajoute une étape et des dépenses non prévues.

Dès que la température le permettra (il fait bien froid au sens du fil), les travaux de restauration reprendront.

## Batterie : le choix du pragmatisme

Grâce aux généreux financements de proches (merci Ben, Aurel et Mathias), nous avons pu acheter les différents composants nécessaires à l'électrification de la 4L.

Par pragmatisme, nous avons décidé d'acheter un bloc batterie déjà éprouvé à savoir une des 7 cellules d'une VW ID3. Elle fait partie des batteries avec la densité énergétique la plus importante et son caisson en aluminium est resistant et ses dimension sont parfaites. Il logera sans problème dans le chassis de la 4L. Evitant ainsi que prendre de la place ailleurs.

En revanche, question chimie, ce n'est pas du Lithium Fer Phosphate comme nous aurions souhaité, mais du Lithium-Manganèse-Cobalt. Il s'agit de celulle produite par LG Pologne, ce sont les mêmes que dans la Renault Zoé.

Donc, de ce côté là rien de bien écologique, si ce n'est le fait qu'au lieu d'embarquer 230kg de ces batteries (soit plus de 45kWh), nous n'en embarquons que 33kg (pour 6,7kWh).
De plus, ce sont des cellules d'occasions, parfait pour la réalisation de notre prototype.

Bien sûr, vous le savez déjà, mais avec une si "petite" batterie, la conviviale n'aura pas l'autonomie des voitures électriques actuelles. C'est un choix assumé, nous voulons concevoir un véhicule qui induit des contraintes à son utilisation et ainsi questionne notre mobilité. La tendance actuelle de développement des véhicules électriques est absolument folle.
Les constructeurs et les politiciens cherchent à nous faire croire que l'on pourra à la fois : remplacer le parc de véhicule thermique par des voitures électriques ayant les mêmes caractéristiques poids/puissance/autonomie, que l'on pourra charger en moins de 30min (je vous dis pas la puissance qu'il faut pour cela) et qu'en même temps on va sortir du nucléaire grâce au développement des énergies renouvellables !
C'est absolument irréalisable et il s'agit clairement d'un mirroir aux alouettes agité à des fins commerciales et électorales...

Nous faisons le choix d'une certaine forme de réalisme et assumons que d'ici quelques années (ou quelques dizaines) la mobilité sera forcément différente. Non pas par choix, mais par contraintes physiques.

Nous gardons comme objectif le fait de pouvoir utiliser des cellules LFP, mais nous n'avons pas trouvé de pack dont les dimensions permettraient de stocker la batterie dans le chassis (qui a une hauteur d'environ 12cm). Et comme dit plus haut, la conception d'un pack de batteries à partir de cellules cylindriques est complexe et ne peut être l'objet de ce prototype.

## Bienvenue au tinyBMS

J'avais rapidement mentionné la problématique du BMS (Battery Management System) dans la newsletter précédente.
C'est un élément crucial dès que l'on utilise des batteries au lithium. En effet, celles-ci peuvent parfois surchaffer ou être en surtension, il faut donc un mécanisme qui permet de couper le courant en cas de problème.
C'est le rôle du BMS. Il protège aussi la batterie de décharges trop profondes.

Les chinois fabriquent toutes sortes de BMS ...

Nous cherchions un BMS qui soit :
- Si possible produit en UE
- Pas trop cher
- Dont le courant ne passe pas dans le circuit (avec un capteur effet HAL)
- Modulable (le port CAN et le bluetooth sont sans doute nécessaire pour le prototype, mais peut-être pas pour la suite)

Grâce à kit voiture elec, nous avons découvert le tinyBMS et j'espère qu'il conviendra. Sont seul inconvénient, il ne peut pas gérer plus de 16 cellules, ce qui limite le nombre de batteries que nous pourrons utiliser.

Espérons que tout fonctionne bien !

