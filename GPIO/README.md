# Exercice 1 : LED 3 états
Dans ce premier exercice nous allons changer l'état de d'une led grâce à un bouton poussoir. Lors de la première pression, la led clignotera. Lorsqu'on appuie une deuxième fois sur le bouton, la led clignote plus vite et une troisième pression éteint la led.

Le code est trouvable [ici](LED_3_States)

Dans ce code, on trouve d'abord la déclaration de nos variables soit le boutton et la led. On a ensuite 4 fonctions dont 3 décriront le comportement de la led (clignotement, clignotement rapide et éteinte) et la dernière permet de passer d'un état à un autre. Enfin, on a la routine d'interruption qui dépend du boutton et la boucle final qui commandera l'état de la led en fonction du mode dans lequel on se trouve.

résultat final :

![gif](https://github.com/HEPL-Dosogne/smartcities/blob/main/GPIO/MicrosoftTeams-video.gif)


# Exercice 2 : Volume d'un buzzer
Ce deuxième exercice se base sur l'utilisation d'un potentiomètre afin de régler le volume d'une mélodie que l'on jouera grâce à un buzzer.
