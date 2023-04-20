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

##LCD - Temp - Humidity - Buzzer

On créé les variables temp et humid qui recevront la valeur lue de la variable dht2 à l'aide de la fonction readTempHumid() qui renvoie la valeur de la température et de l'humidité.

Ensuite on procède de la même manière que les fois précédente pour afficher les valeurs à l'écran. On clear(), définit la position du curseur pour l'affichage de chaque valeur à l'aide de setCursor(). setCursor(0,0) défini la première ligne et première colonne qui désigne la case à partir de laquelle le message contenant la valeur de "Temp" s'affichera. On convertit à nouveau cette valeur sous forme de string pour qu'elle soit affichable par la fonction "print()" à l'aide la fonction "str()".

On reproduit la même manipulation pour la valeur de Humid qui sera affichée sur la 2ème ligne grace à setCursor(0,1).

On créé ensuite une condition "if" et "else" pour faire sonner le buzzer lorsque la valeur de temp est supérieur à 30 ou que la valeur de humid est inférieure à 20. Sinon le buzzer ne fait pas de bruit.






