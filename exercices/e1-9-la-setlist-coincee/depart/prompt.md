# Prompt — setlist coincée

Voici mon HTML/JS (je colle le fichier).

Ce que je veux : pouvoir glisser une ligne de la liste pour changer l’ordre
(horaires du plus tôt au plus tard). Pas de librairie. Pas de nouvelle page.

Ce que je vois quand je glisse :
Je peux prendre une ligne, mais quand je la dépose ailleurs, elle ne change pas de place.
Le curseur indique que le dépôt n’est pas autorisé et la ligne revient à sa place.

Ce que dit la console (F12) :
La console affiche « prise : ... » au moment où je commence à glisser,
mais je ne vois pas de message « dépôt, id reçu : ... ».

Explique d’abord le concept du glisser-déposer HTML :
quels événements, dans quel ordre, et pourquoi dragover a souvent besoin
de preventDefault.

Liste ensuite les problèmes de CE fichier (pas d’un exemple inventé).

Propose ENSUITE le plus petit changement possible.
Ne réécris pas toute la page.

# remqrques après correction : 
Le glisser-déposer utilise plusieurs événements : dragstart quand on prend une ligne, dragover quand on la survole et drop quand on la dépose.

Il faut autoriser le dépôt avec preventDefault() pendant dragover et utiliser le même type de donnée pour écrire puis relire l’identifiant dans dataTransfer.

Dans ce fichier, il fallait aussi viser la ligne <li> avec closest("li"), sinon le dépôt pouvait viser un élément à l’intérieur de la ligne.