## LCD - Temp - Humidity - Buzzer

On utilise le capteur DHT11 d'humidité et de tempérture.

On créé les variables temp et humid qui recevront la valeur lue de la variable dht2 à l'aide de la fonction readTempHumid() qui renvoie la valeur de la température et de l'humidité.

Ensuite on procède de la même manière que les fois précédente pour afficher les valeurs à l'écran. On clear(), définit la position du curseur pour l'affichage de chaque valeur à l'aide de setCursor(). setCursor(0,0) défini la première ligne et première colonne qui désigne la case à partir de laquelle le message contenant la valeur de "Temp" s'affichera. On convertit à nouveau cette valeur sous forme de string pour qu'elle soit affichable par la fonction "print()" à l'aide la fonction "str()".

On reproduit la même manipulation pour la valeur de Humid qui sera affichée sur la 2ème ligne grace à setCursor(0,1).

On créé ensuite une condition "if" et "else" pour faire sonner le buzzer lorsque la valeur de temp est supérieur à 30 ou que la valeur de humid est inférieure à 20. Sinon le buzzer ne fait pas de bruit.
## LCD - Temp - Humidity - Buzzer

On créé les variables temp et humid qui recevront la valeur lue de la variable dht2 à l'aide de la fonction readTempHumid() qui renvoie la valeur de la température et de l'humidité.

Ensuite on procède de la même manière que les fois précédente pour afficher les valeurs à l'écran. On clear(), définit la position du curseur pour l'affichage de chaque valeur à l'aide de setCursor(). setCursor(0,0) défini la première ligne et première colonne qui désigne la case à partir de laquelle le message contenant la valeur de "Temp" s'affichera. On convertit à nouveau cette valeur sous forme de string pour qu'elle soit affichable par la fonction "print()" à l'aide la fonction "str()".

On reproduit la même manipulation pour la valeur de Humid qui sera affichée sur la 2ème ligne grace à setCursor(0,1).

On créé ensuite une condition "if" et "else" pour faire sonner le buzzer lorsque la valeur de temp est supérieur à 30 ou que la valeur de humid est inférieure à 20. Sinon le buzzer ne fait pas de bruit.

## Intelligent Fan

cette fois on utilise l'écran pour n'afficher qu'une seule variable, temp.

on créé également une condition if - else dans une boucle "while True".
Si la valeur de la température est supérieur à 26, on active le ventilateur à l'aide de la fonction value() qui attribue un état haut ou bas en fonction de si l'on place un 1 ou un 0 dans ses parenthèses. au préalable la variable minifan aura été créé pour lui affecter une valeur.


![20230410_151906](https://user-images.githubusercontent.com/129083868/233367649-5dc58f57-259d-4308-988e-d583c0311765.jpg)
![20230410_151933](https://user-images.githubusercontent.com/129083868/233367665-60bd26bc-9cde-4891-b4f1-4850273237ac.jpg)
![20230410_151937](https://user-images.githubusercontent.com/129083868/233367670-4fe912f7-8eb3-4ca5-8f1c-ff74b988ef06.jpg)


