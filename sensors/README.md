# Exercice 3 : Contrôle de la température
Dans ce troisième exercice, nous allons créer un programme qui permet de gérer un thermostat à plusieurs états. Nous allons afficher sur notre écran LCD la température mesurée par notre capteur de température ainsi qu'une température de consigne. 

Lorsque la température de la pièce ne dépasse pas la température de consigne, on affiche simplement la température. 

Le deuxième état se déclanche lorsque la température mesurée dépassse la température de consigne. Alors, une led se met à clignoter à une fréquence de 0,5Hz. 

Le dernier état se produit lorsque la température ambiente dépasse la température de consigne de + de 3°C.
Lorsque ça arrive, un buzzer émettra une certaine fréquence pour prévenir l'utilisateur, la led clignotera plus vite et le mot "ALARM" apparaitra à l'écran (Nous verrons deux possibilités différentes : faire clignoter le mot alarm ou le faire défiler sur notre écran)

Pour réaliser un tel exercice, nous utiliserons les commandes présentes dans la librairie du lcd qui est trouvable [ici] (

Le code est trouvable [ici]


résultat final :

![gif](https://github.com/HEPL-Dosogne/smartcities/blob/main/GPIO/MicrosoftTeams-video.gif)

