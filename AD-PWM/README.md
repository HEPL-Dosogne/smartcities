# Exercice 2 : Volume d'un buzzer
Ce deuxième exercice se base sur l'utilisation d'un potentiomètre afin de régler le volume d'une mélodie que l'on jouera grâce à un buzzer. En plus de ça, on rajoute un boutton poussoir qui permet de passer d'une mélodie à une autre. On incluera aussi une led qui cignotera sur le rythme de la musique dans la version améliorée du code

## Version 1 
Le code est [ici](BuzzerV1)

Dans cette première version, on crée une fonction pour chacune de nos notes ainsi qu'une 8e qui sera utilisée comme un silence. Chaque fonction est directement dépendante du temps (pendant laquelle on veut jouer la note) ainsi que d'une variable volume déterminée par notre potentiomètre (fonction Update_Vol()). 
Viens ensuite nos deux fonctions mélodies dans lesquelles on utilises les fonctions notes pour créer une mélodie. Enfin, on utilisé une routine d'interruption en fonction du boutton afin de passer de la mélodie 1 à 2 grâce à celui-ci.

## Version 2
le code est [ici](BuzzerV2)

Dans cette deuxième version, on utilise des listes pour définir nos notes et nos mélodies. Plus besoin d'une fonction pour chaque note utilisée. On garde cependant la fonction pour le volume et la routine d'interruption liée au boutton. A celles-ci vient se rajouter la fonction "Play(note,time)" qui va nous permettre de jouer chaque notes, une par une, en parcourant les listes prédéfinies.
On a aussi rajouter dans cette version, une led clignotant au même rythme que la mélodie jouée (inclu dans la fonction Play)

## Hardware

![image](https://github.com/HEPL-Dosogne/smartcities/blob/main/AD-PWM/Buzzer.png)


Une amélioration intéressante serait de permettre au boutton de changer de mélodie immédiatemment lorsqu'on appuie dessus. Dans les 2 cas présentés ci-dessus, le changement se fait lorsque la mélodie actuelle est terminée.
