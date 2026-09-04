# Journal du jeu du prompt
## Manche 1 — trop vague
Prompt : change le bouton
Ce que l’IA a fait : le bouton reste gris au départ et devient rouge après le clic, sans JavaScript.
Pourquoi c’est un problème : pas de problème ?
## Manche 2 — précis
Prompt : (celui du cours)
Résultat : le bouton devient orange au clic 
Explication que je retiens :
-  La ligne bouton.addEventListener "click", function () écoute le clic sur le bouton.
- La ligne bouton.style.backgroundColor = "#e36414"; change son fond en orange, et la ligne suivante met le texte en blanc.
- On a besoin de l’id "magic" pour que JavaScript puisse retrouver précisément ce bouton dans la page avec getElementById("magic").
- L'ia n'a pas modifié le titrem paragraphe ou le CSS exsitant
## Ce que je changerais la prochaine fois
- faire des demandes précises à l'ia
