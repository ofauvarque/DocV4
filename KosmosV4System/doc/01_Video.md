# Intégration mécanique & électronique interne

## Impression de la structure 3D

Imprimer la structure mécanique à l'aide d'une imprimante 3D filaire.

<img src="pictures/V4_Video/Structure.PNG" height=300>

## Fixation du capteur d'ambiance lumineuse RGB

- Souder le connecteur JST 4 pin sur les bornes GND 3.3V SDA SCL de la carte électronique du capteur. (La borne INT est inutilisée.) ATTENTION, les soudures se font du côté du capteur lumineux.

<img src="pictures/V4_Video/IMG_1317.JPG" height=200> <img src="pictures/V4_Video/IMG_1321.JPG" height=200>

- Sur la structure mécanique, préformer les deux trous destinés à accueillir le capteur à l'aide d'un boulon de diamètre 2.5 mm.
- Fixer le capteur sur la structure mécanique à l'aide de boulons de diamètres 2.5 mm et de longueur 6 mm. (Des boulons plus longs peuvent être utilisés mais ils ne doivent pas dépasser de la structure.)

<img src="pictures/V4_Video/IMG_1322.JPG" height=200> <img src="pictures/V4_Video/IMG_1323.JPG" height=200>

## Fixation de la caméra
Pour un rendu de couleurs proche de celui de l'oeil humain, le capteur Picam HQ est équipé d'un filtre infra-rouge se matérialisant par une petite vitre bleue-verte devant le capteur. Ce filtre en plus de couper les infrarouges, atténue également une partie de la lumière rouge. Or celle-ci est déjà fortement atténuée par l'eau de mer. Afin d'éviter une telle perte inutile, le filtre IR du capteur Picam de KOSMOS doit être enlevé. Pour ce faire, un excellent tutoriel existe sur le site officiel de raspberry :  

https://www.raspberrypi.com/documentation/accessories/camera.html#ir-filter

A l'issue de cette opération, on obtient un capteur Picam HQ sans filtre IR (qui n'aura plus d'utilité par la suite).

<img src="pictures/V4_Video/11.jpeg" height=200> <img src="pictures/V4_Video/9.jpeg" height=200>

- Oter également le support de la vis caméra.

<img src="pictures/V4_Video/IMG_1326.JPG" height=200> 

- Fixer la capteur caméra sur la structure à l'aide de 4 boulons (diamètre 2.5 mm  et longueur 10 mm) et de 4 écrous. Attention à respecter l'orientation de la carte. 

<img src="pictures/V4_Video/IMG_1327.JPG" height=200> <img src="pictures/V4_Video/IMG_1328.JPG" height=200> <img src="pictures/V4_Video/IMG_1329.JPG" height=200> 

## Fixation de la Raspberry Pi 

- Fixer les radiateurs sur la carte RPi.  Connecter ensuite le RTC à la RPi via le port BAT. Fixer la pile du RTC au dessus du port Ethernet avec le double face fourni avec le RTC. 

<img src="pictures/V4_Video/19_2.jpeg" height=200> <img src="pictures/V4_Video/19.jpeg" height=200> <img src="pictures/V4_Video/IMG_13300.JPG" height=200>

- Assembler 4 boulons (diamètre 2.5 mm et longueur 10 mm) et 4 écrous sur chacun des trous de la RPi de la structure mécanique. Les écrous permettront de surélever légèrement la carte.

<img src="pictures/V4_Video/IMG_1330.JPG" height=400> <img src="pictures/V4_Video/IMG_1331.JPG" height=400> <img src="pictures/V4_Video/IMG_1332.JPG" height=400>

- Positionner la carte RPi et la fixer avec deux écrous dans les coins avant droit et arrière gauche et avec deux entretoises  (diamètre 2.5 mm, hauteur 20 mm) dans les coins avant gauche et arrière droit. Connecter ensuite la nappe entre le capteur vidéo et la carte RPi.

<img src="pictures/V4_Video/IMG_1332.JPG" height=400> <img src="pictures/V4_Video/IMG_1333.JPG" height=400>

- Insérer la clé USB dans un des deux ports USB 3.0

## Réalisation de la carte électronique

<img src="pictures/V4_Video/IMG_0625.JPG" height=200> <img src="pictures/V4_Video/IMG_0626.JPG" height=200>

<img src="pictures/V4_Video/20250225_141010.jpg" height=300> <img src="pictures/V4_Video/IMG_1571.jpg" height=300> <img src="pictures/V4_Video/IMG_1572.jpg" height=300>

<img src="pictures/V4_Video/IMG_1610.JPG" height=200> <img src="pictures/V4_Video/IMG_1611.JPG" height=200>






# Réalisation du caisson étanche

<img src="pictures/V4_Video/VueGenerale.PNG" height=400>

## Assemblage du hublot sphérique

## Assemble du bouchon arrière

### Cable d'alimentation

- Avec une pince coupante, raccourcir le cable COB-1231 pour qu'il mesure 40 cm. Garder les fils noir, jaune et rouge. 
- Avec un cutter, enlever 10 cm de gaine noire. Attention à ne pas abimer les fils à l'intérieur. (Si c'était le cas glisser de la gaine thermoretractable au niveau de la coupure.)
- Couper le fil rouge à ras de la gaine pour ne conserver que le noir et le jaune. (On rappelle la convention : 5V jaune, masse noir, 12V rouge.)
- Dénuder les fils jaune et noir sur 7 mm.
- Y sertir des cosses dont on a vérifié qu'elles avaient le diamètre optimal.

<img src="pictures/V4_Video/FlexibleAlimentation.jpeg" height=300> <img src="pictures/V4_Video/IMG_1495.jpg" height=300>

- Suivre ensuite le tutoriel dont le lien est ci-dessous pour installer le presse étoupe

https://bluerobotics.com/learn/wetlink-penetrator-installation-guide/

https://www.youtube.com/watch?v=vigY82tsfOI&t=2s&ab_channel=BlueRobotics

<img src="pictures/V4_Video/IMG_1769.jpg" height=200> <img src="pictures/V4_Video/IMG_1770.jpg" height=200>

### Assemblage de la tape connectique

<img src="pictures/V4_Video/TapeArriere.PNG" height=400>

- Graisser les joints de chaque éléments sur la bouchon 7 trous
- Serrer les éléments M10 sur le bouchon en suivant l'ordre indiqué sur la figure.
    
<img src="pictures/V4_Video/IMG44.jpg" height=400> <img src="pictures/V4_Video/IMG19.jpg" height=400>

### Connectiques 

- Sur le connecteur 4 pin Power Bulkhead COB-1140, raccourcir les cables pour qu'ils mesurent 10 cm.
- Dénuder les fils sur 5 mm puis y sertir des cosses JST. Vérifier qu'elles tiennent fermement.

<img src="pictures/V4_Video/1.jpeg" height=200> 
 
- De la même façon, couper les cables du capteur Température Pression pour qu'ils mesurent 10 cm.
- Dénuder les fils sur 3 mm puis y sertir les cosses.
- Re-écraser les mords à la pince plate pour que les cosses tiennent fermement. (Les fils du capteur TP sont un peu fins pour les cosses.) 
- Insérer les cosses dans les connecteurs JST en suivant le plan de cablage.

<img src="pictures/V4_Video/IMG_E1626.JPG" height=300> <img src="pictures/V4_Video/IMG_E1624.JPG" height=300>

- Sur le connecteur 8 pin Power Bulkhead COB-1180, raccourcir les cables pour qu'ils mesurent 7cm et sertir un connecteur ethernet en respectant le code couleur suivant.

<img src="pictures/V4_Video/Ethernet.PNG" height=200>

## Réalisation du cable de récupération des données

<img src="pictures/V4_Video/Ethernet.PNG" height=200> <img src="pictures/V4_Video/RecupDonneesCable.PNG" height=200>  

# Assemblage final


### Fixation de l'antenne GPS

- A l'aide d'un pistolet à colle fixer l'antenne comme indiqué sur la photo suivante.
- La brancher ensuite sur le capteur GPS présent sur la carte électronique.

<img src="pictures/V4_Video/IMG_1339.JPG" height=300>

### Connexion du capteur de luminosité

- Couper 6 cm de fils rouge, noir, blanc et vert et sertir des connecteurs JST de chaque côté.
  
- Les insérer dans des connecteurs 4 pin en respectant l'ordre de couleurs de la photo suivante.

<img src="pictures/V4_Video/IMG_1341.JPG" height=300>

- Brancher ce connecteur entre la carte électronique et le capteur de luminosité.

### Fixation de la tape arrière

- Fixer la tape arrière sur la structure mécanique à l'aide de 4 boulons (diamètre 3 mm, longueur 10 mm). On placera le détrompeur de la tape du côté des ports USB 2.0 



### Connexion l'

