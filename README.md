# Régression linéaire multiple

## Présentation

Pour cela nous allons réaliser une régression linéaire multiple (expliquer une donnée quantitative par des données quantitatives).
Le test de saut RSI est réalisé le premier jour de la semaine suivant le match, nous allons procédér à une première manipulation des données (plusieurs bases de données à croiser) afin de garder les données les plus consistantes (ne pas dépasser 3 jours entre le match et le saut).

## Conclusion

Les coefficients et les intervalles sont des nombres très petits de par les valeurs petites du RSI et les grandes valeurs des différentes variables GPS. Egalement le RSI a une variabilité assez faible.
A noter que le modèle a un R² de 0.103 donc le modèle explique 10.3% de la variabilité du RSI.

De plus, le modèle nous confirme des choses que nous savons déjà par expérience : les efforts intenses (à dominante neurale) vont avoir plus d'impact sur le score RSI (obtenu d'un effort neural également). Il est tout de même intéressant de noter que les décelérations auraient un effet positif sur le score RSI.

Enfin, pour conclure, la principale limite de la méthode et des conclusions est que nous ne prenons pas en compte l'environnement du sportif entre le match et le saut : les deux étant séparés entre 2 et 3 jours, la qualité de vie, récupération etc. du sportif vont beaucoup jouer sur sa qualité de saut réalisé en début de semaine.

(Et ici la base de données manque de consistance : beaucoup de joueurs avec une seule saisie, seulement 3 joueurs avec 8 saisies...).

## Perspectives

Pour être plus précis et espérer avoir un modèle plus performant, nous pourrions nous procurer davantage de données des matchs comme : la durée de jeu, des données sur les contacts (nombre et intensité), découper en zone d'intensité (km/h, m.s-²) les efforts intenses (sprints, accélérations, décelérations) ou encore une information sur le match (domicile ou extérieur, moyen de transport).

Nous pourrions analyser chaque joueur avec suffisamment de données individuelles ou encore par groupes (avants et arrières).

Enfin, nous pourrions nous intéresser aux composantes du RSI dans le modèle de régressions multiple. Car ce score est un ratio ou un produit (selon le calcul, https://www.scienceforsport.com/reactive-strength-index/). Il serait donc plus intéressant de savoir quelle composante peut être le mieux expliquée par les données de match.
