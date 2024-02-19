# Exercice 2 : Volume d'un buzzer
Ce deuxième exercice se base sur l'utilisation d'un potentiomètre afin de régler le volume d'une mélodie que l'on jouera grâce à un buzzer. En plus de ça, on rajoute un boutton poussoir qui permet de passer d'une mélodie à une autre. On incluera aussi une led qui cignotera sur le rythme de la musique dans la version améliorée du code

## Version 1
Le code est [ici](BuzzerV1)

Dans cette première version, on crée une fonction pour chacune de nos notes ainsi qu'une 8 qui sera utilisé comme un silence. Chaque fonction est directement dépendante du temps (pendant laquelle on veut jouer la note) ainsi que d'une variable volume déterminée par notre potentiomètre (fonction Update_Vol()). 
Viens ensuite nos deux fonctions mélodies dans lesquelles on utilises les fonctions notes pour créer une mélodie. Enfin, on utilisé une routine d'interruption en fonction du boutton afin de passer de la mélodie 1 à 2 grâce à celui-ci 
