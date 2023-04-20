# LCD 
Pour pouvoir utiliser l'écran lcd il est nécessaire d'utiliser 2 librairies de code. La première étant [lcd1602](Lib/LCD1602) qui sert à controler l'écran lcd et la 2ème qui est I2C et qui permet la communication des données entre l'écran et le pico w.

## Hello World

Programme basique pour afficher un message à l'écran. 
on définit une variable qui reprend les caractéristiques de l'écran LCD en définissant le nombre de ligne et colonne ainsi que le type de communication.
Ensuite on utilise les fonctions suivante:
display() pour activer l'affichage
clear() pour nettoyer l'affichage.
print() pour afficher le message sur l'écran.
setCursor() pour positioner le curseur sur une ligne et une colonne et donc définir la case à partir de laquelle le message commence à s'afficher.

##Affichage des valeurs du Potentiomètre.

Afin d'utiliser le potentiomètre qui renvoie des valeurs analogiques, il est nécessaire d'utiliser la librairie ADC qui s'utilise comme la librairie Pin servant à spécifier sur quel connecteur la communication se fait.

A nouveau, on définit une variable qui reprend les caractéristiques de l'écran LCD en définissant le nombre de ligne et colonne ainsi que le type de communication.
Ensuite on utilise les fonctions suivante:
display() pour activer l'affichage
clear() pour nettoyer l'affichage.
print() pour afficher le message sur l'écran.
setCursor() pour positioner le curseur sur une ligne et une colonne et donc définir la case à partir de laquelle le message commence à s'afficher.

afin d'afficher la valeur analogique du potentiomètre au travers de la fonction print(), il est nécessaire de convertir cette valeur en un string à l'aide de la fonction str().





