# Comment ça function… L'animation de chargement de Gmail

Une animation de chargement super légère pour un webmail super lourd ? C'est possible et voici comment ça function…

En avril 2018, Google a mis à jour le webmail desktop de Gmail. Et le premier truc qui m'a sauté aux yeux, c'est l'écran de chargement. On est passé d'une barre de progression basique à une belle animation de chargement.

J'ai d'abord pensé que c'était un GIF animé, ou alors une vidéo, voire même un WebP animé puisqu'on est chez Google.

Et puis je me suis souvenu d'une technique utilisée par Google pour certains doodles au début des années 2010. TK

Eh bien en fait… rien de tout ça.

## Message

L'animation de chargement de Gmail est dessinée en CSS. Et la barre de progression est complètement bidon.

## Accroche / amorce

* Redesign de Gmail en 2018. Je me suis demandé comment c'était fait.
* 150 fichiers pour plus de 10 Mo non compressés (contre 40 Ko pour le tout premier Gmail)

## Structure

1. GIF? MP4?
2. [Doodle](https://www.google.com/doodles/4th-of-july-2010-and-rube-goldbergs-birthday) et [Crushinator](https://www.youtube.com/watch?v=EqEqGK3uRN8).
3. Dessin en CSS !
4. La barre de progression ? Juste une animation CSS de 12 secondes. Elle n'indique en rien la progression.

## Ajout de rythmes possibles

1. fun fact
2. blague
3. effet spécial
4. manipulation

## Doit absolument être dans la vidéo

* …

## “Nice to have”

* Anime : https://www.youtube.com/watch?v=4M2wcyezJT0
* Cute : https://blog.prototypr.io/how-i-started-drawing-css-images-3fd878675c89?gi=5e15392df35b
* Single div : https://hacks.mozilla.org/2014/09/single-div-drawings-with-css/
* Mustache : https://codepen.io/miocene/pen/mjLPVp
* Francine : http://diana-adrianne.com/purecss-francine/
* Lemon glass : https://codepen.io/ivorjetski/full/xMJoYO
* [Mon tweet de base](https://twitter.com/HTeuMeuLeu/status/989502931295768576)
* [Le code de l'animation](https://cdn.rawgit.com/hteumeuleu/10e89de83f362646e2e12365308440f8/raw/f69d62eba19f0c743c5590cc0146c00a670ea58e/gmail-animation.html)

## Description

## Miniatures

* Une capture d'écran de l'animation de Gmail en fond. Avec une flèche rouge et un text qui dit "FAKE?".

---

## Ancien script

En avril 2018, Google a mis à jour Gmail en lançant le plus gros redesign du webmail depuis 2011. Au fil des années, le webmail est devenue une grosse usine bourrée de JavaScript qui va jusqu'à charger plus de 150 fichiers pour plus de 10 Mo non compressés au total. On est loin, très loin, de la douzaine de requêtes et des 40 Ko de la toute première version de Gmail.

Gmail affiche un écran de chargement dédié. Et le premier truc que j'ai remarqué lors de la refonte, c'est ce nouvel écran de chargement. On est passé d'une simple barre de progression à une animation bien chiadée. Je me suis tout de suite demandé comment c'était fait. J'ai d'abord pensé que c'était une vidéo, ou alors un gros sprite comme l'a souvent fait Google pour ses Doodles. Et c'est là que je me suis rendu compte que toute cette animation est faite juste en HTML et CSS.

La pratique de dessiner en HTML et CSS n'est pas récente. Ça se faisait déjà avec des tableaux en HTML.

La plupart du temps, ces dessins sont purement expérimentaux. Et c'est vraiment un chouette exercice pour appréhender certaines notions de HTML et CSS. Mais c'est assez rare de trouver des exemples de dessin comme ça dans la vraie vie. Et encore moins dans un service qui compte un milliard et demi d'utilisateurs comme Gmail. Alors voici comment ça function.
