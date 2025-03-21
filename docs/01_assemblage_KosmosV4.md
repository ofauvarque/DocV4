# Assemblage KOSMOS version 4
<details open>
  <summary> Sommaire </summary>
  
  1. [Assemblage du caisson vidéo](assemblage_µkosmos.md#1-assemblage-du-boitier-électronique)
  2. [Assemblage du caisson batterie](assemblage_µkosmos.md#2-assemblage-du-caisson-vid%C3%A9o)
  3. [Assemblage du caisson moteur](assemblage_µkosmos.md#3-assemblage-du-tr%C3%A9pried)
      
</details>

## 1. Assemblage du caisson vidéo
<details>
  <summary> Outils </summary>
  
  * gaine thermo {[Etape 1](assemblage_µkosmos.md#etape-1---réaliser-les-raccordements-entre-les-câbles-et-les-connecteurs)}
  * matériel soudure {[Etape 1](assemblage_µkosmos.md#etape-1---réaliser-les-raccordements-entre-les-câbles-et-les-connecteurs)}
  * couronne de forage (diamètre:...) {[Etape 3](assemblage_µkosmos.md#etape-3---percer-les-côtés-du-boitier)}
  * foret (diametre: ..) {[Etape 3](assemblage_µkosmos.md#etape-3---percer-les-côtés-du-boitier)}
  * perceuse {[Etape 3](assemblage_µkosmos.md#etape-3---percer-les-côtés-du-boitier)}
  * velcro {[Etape 4 et 5](assemblage_µkosmos.md#etape-4---fixer-le-receiver-gaming-la-carte-gps-et-le-ventilateur-dans-la-boite)}
  * tourne vis plat 
  * tourne vis cruciforme
  
</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel caisson vidéo](/../µKOSMOS/hardware/02_materiel_boitier_electronique.md)
    
</details>

### Vue générale

<img src="pictures/V4_Video/VueGenerale.jpeg" height=400>

### Pose des radiateurs sur la Raspberry Pi

- Mettre les radiateurs sur les puces de la RPi.

<img src="pictures/V4_Video/18.jpeg" height=400>

- Connecter ensuite le RTC à la RPi via le port BAT. Fixer la pile du RTC au dessus du port Ethernet avec du Velcros. 

### Modification du capteur Picam HQ

Pour un rendu de couleurs proche de celui de l'oeil humain, le capteur Picam HQ est équipé d'un filtre infra-rouge se matérialisant par une petite vitre bleue-verte devant le capteur. Ce filtre en plus de couper les infrarouges, atténue également une partie de la lumière rouge. Or celle-ci est déjà fortement atténuée par l'eau de mer. Afin d'éviter une telle perte inutile, le filtre IR du capteur Picam de KOSMOS doit être enlevé. Pour ce faire, un excellent tutoriel existe sur le site officiel de raspberry :  

https://www.raspberrypi.com/documentation/accessories/camera.html#ir-filter

A l'issue de cette opération, on obtient un capteur Picam HQ sans filtre IR (qui n'aura plus d'utilité par la suite).

<img src="pictures/V4_Video/9.jpeg" height=200>

### Préparation de la vis de fixation de la caméra

La vis de fixation de la caméra a initialement un arceau métallique facilitant son serrage. Cet arceau, trop encombrant dans le caisson doit être ôté à l'aide d'une pince coupante.  

<img src="pictures/V4_Video/8.jpeg" height=200> <img src="pictures/V4_Video/7.jpeg" height=200>

### Réalisation du cable d'alimentation

- Avec une pince coupante, raccourcir le cable COB-123P1 pour qu'il mesure 40 cm. Garder les fils noir, blanc et rouge. La gaine ne sera plus utilisée.
- Avec un cutter, enlever 10 cm de gaine noire. Attention à ne pas abimer les fils à l'intérieur. (Si c'était le cas glisser de la gaine thermoretractable au niveau de la coupure.)
- Couper le fil rouge à ras de la gaine pour ne conserver que le noir et le blanc. (On rappelle la convention : 5V Blanc et Noir. 12 V Rouge et Noir.)
- Dénuder les fils blancs et noir sur 7 mm.
- Y sertir des cosses dont on a vérifié qu'elles avaient le diamètre optimal.

<img src="pictures/V4_Video/FlexibleAlimentation.jpeg" height=400> <img src="pictures/V4_Video/IMG_1495.jpg" height=400>


https://bluerobotics.com/learn/wetlink-penetrator-installation-guide/

https://www.youtube.com/watch?v=vigY82tsfOI&t=2s&ab_channel=BlueRobotics

### Connectiques caisson

- Sur deux connecteurs 4 pin Power Bulkhead COB-1140-SS et raccourcir les cables pour qu'ils mesurent 10 cm.
- Dénuder les fils sur 5 mm puis y sertir des cosses JST. Vérifier qu'elles tiennent fermement.
- De la même façon, couper les cables du capteur Température Pression pour qu'ils mesurent 10 cm.
- Dénuder les fils sur 3 mm puis y sertir les cosses. Les mords doivent prendre sur la gaine plastique des fils. 
- Re-écraser les mords à la pince plate pour que les cosses tiennent fermement. (Les fils du capteur TP sont un peu fins pour les cosses.)
- AVANT d'INSERER LES COSSES DANS LEUR CONNECTEUR JST, passer les cables des trois éléments dans le bouchon à 7 trous.
 
<img src="pictures/V4_Video/IMG_1567.jpg" height=400>

- Insérer les cosses dans les connecteurs JST en suivant le plan de cablage.

### Réalisation de la carte électronique

<img src="pictures/V4_Video/20250225_141010.jpg" height=400>

### Assemblage des éléments

- Fixer la nappe et l'objectif à la caméra

<img src="pictures/V4_Video/IMG20250122142122.jpg" height=400>

- Fixer les entretoises à la Raspberry Pi dans les coins visibles sur la photo qui suit.
- Fixer la carte Raspberry Pi à la structure interne du caisson imprimée en 3D dans les deux coins restants.

<img src="pictures/V4_Video/IMG20250122142746.jpg" height=400> <img src="pictures/V4_Video/12.jpeg" height=400>

- Fixer la caméra sur la structure 3D.
- Relier la nappe à la Raspberry Pi.
- Placer la carte électronique sur la Raspberry Pi et la fixer aux entretoises.

 


## Assemblage du caisson batterie

### Cable de recharge 

<img src="pictures/V4_Batterie/Chargeur.jpeg" height=400>


- A l'aide de la petite clé fournie avec le chargeur, régler le transformateur sur 13.5 V
  
<img src="pictures/V4_Batterie/20.jpeg" height=400>

- Avec une pince coupante, raccourcir le cable COB-123P1 pour qu'il mesure 20 cm.
- Avec un cutter, enlever 5 cm de gaine noire. Attention à ne pas abimer les fils à l'intérieur. (Si c'était le cas glisser de la gaine thermoretractable au niveau de la coupure.)
- Raccourcir de 1 cm le morceau de gaine noire et le fendre dans la longueur.
- Enfiler 5 cm de gaine thermoretractable sur la gaine noire
- Dénuder les fils rouge et noir sur 5 mm.
- Enfiler un morceau de gaine thermoretractable de 2 cm sur chacun de ces deux fils en choississant leur diamètre afin qu'il puisse recouvrir la cosse du connecteur XT60 femelle.
- Souder les fils rouge et noir sur le connecteur XT60 en respectant les polarités : + sur rouge et - sur noir.
- Faire glisser les gaines thermoretractables et les chauffer.
- Englober les trois fils noir rouge et blanc (non soudé) avec la gaine fendue. Remonter la gaine thermorétractable et la chauffer. 

<img src="pictures/V4_Batterie/14.jpeg" height=200> 

- Souder deux cables rouge et noir de 10 cm (récup', comme ceux des multimètres) sur un connecteur XT60 mâle en respectant la polarité.
- De l'autre côté, dénuder ces cables sur 3mmn, les étamer et les souquer dans le connecteur femelle fourni avec le chargeur. 

<img src="pictures/V4_Batterie/1.jpeg" height=200>

<img src="pictures/V4_Batterie/13.jpeg" height=400>


### Vue générale de l'étanchéité

<img src="pictures/V4_Batterie/VueGenerale.jpg" height=400>

<img src="pictures/V4_Batterie/Bouchon.jpg" height=200>


### Vue générale de l'électronique interne

<img src="pictures/V4_Batterie/CarteBatterie.jpeg" height=400> 

- Couper les connectiques originales de l'interrupeur pour les remplacer par des cosses à sertir.
- Tordre les pattes de l'interrupteur à 90° (pour des raisons de compacité)

<img src="pictures/V4_Batterie/SwitchOrigine.jpeg" height=150> <img src="pictures/V4_Batterie/SwitchCoupe.jpeg" height=150> 

- Sur deux connecteurs 3 pin Power Bulkhead COB-113P0-SS et raccourcir les cables pour qu'ils mesurent 10 cm.
- Sur l'un d'eux couper à ras le fil blanc, sur l'autre couper à ras le fil rouge. Le premier fournira du 5V pour le caisson vidéo, le second du 12V pour le caisson moteur.
- AVANT DE SOUDER LES CONNECTEURS XT30, visser ces deux connecteurs sur le bouchon à 4 trous.  

<img src="pictures/V4_Batterie/ConnectiqueCaisson.jpeg" height=400>  

- Sur les fils issus des connecteurs 3 pin Power Bulkhead, souder des XT30 mâle en respectant la polarité. Distinguer le 5V (Noir&Blanc) et le 12V (Noir&Rouge) avec des gaines thermoretractables de couleurs différentes.

<img src="pictures/V4_Batterie/5.jpeg" height=200>  

- Réaliser un raccord "XT30 femelle vers cosses à sertir" de 10 cm pour des fils noir et blanc. (Les récupérer du raccoucissement des cables COB-123P1 et COB-1241.)

<img src="pictures/V4_Batterie/6.jpeg" height=150>

- Réaliser un second raccord "XT30 femelle vers cosses à sertir" pour les fils noir et rouge mais repartir de ces cosses vers d'autres cosses. On choisira pour cela des cosses suffisamment larges pour y insérer deux cables à la fois. 

<img src="pictures/V4_Batterie/7.jpg" height=300>  <img src="pictures/V4_Batterie/8.jpeg" height=300>  

- Réaliser un raccord "XT60 mâle vers cosses à sertir" avec des cables noir et rouge. 

<img src="pictures/V4_Batterie/IMG_156.jpg" height=150>  

### Réalisation de la batterie



<img src="pictures/V4_Batterie/ElectroniqueBatterie.jpeg" height=200>

<img src="pictures/V4_Batterie/FilsBatterieOrigine.jpeg" height=100>

<img src="pictures/V4_Batterie/FilsBatterieCoupe.jpeg" height=100>

<img src="pictures/V4_Batterie/IMG_15.jpg" height=150>  





### Installation Soft Arduino Moteur

- Installer le logiciel Arduino depuis le site https://www.arduino.cc/en/software
- Télécharger control_motor.ino depuis le github [KonkArLAb/kosmos_software le mettre dans un dossier du même nom](https://github.com/KonkArLab/kosmos_software/tree/dev_stereo_merge_imt)
- Placer ce fichier .ino dans un dossier nommé control_motor
- Lancer l'IDE Arduino et ouvrir control_motor.ino
- Brancher l'Arduino Nano à l'ordinateur via le port USB
- Effectuer l'installation demandée par l'IDE Arduino
- Dans l'onglet Tools, sélectionner le port COM auquel est branché l'Arduino Nano
- Dans l'onglet Tools, sélectionner la board Arduino Nano
- Dans l'onglet Tools, Manage Librairie. Taper "AccelStepper". Installer la librairie associée.
- Vérifier le code.
- Téléverser.


### Relier un câble USB à un câble micro USB en passant par le commutateur 

> [!NOTE]
> Ce câble fera le lien entre la batterie et la Raspberry et permetta d'alimenter la carte. Le commutateur permet de couper le courant sans débrancher les câbles.

- couper le câble USB à une trentaine de centimètre du branchement USB  
- enfiler la gaine thermo sur le câble (elle sera chauffée à la fin)  
- utiliser les connecteurs cosses pour faire le lien entre les pins du commutateur et le câble USB, brancher le fil noir et le fil rouge  
- chauffer la gaine thermo pour recouvrir tous les fils  
- répéter les mêmes étapes que pour le côté avec le câble micro USB et le commutateur

<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/ceec4b8716ca7170e905918eca46779770e4e37d/docs/pictures/assembly_guide/commutateur_cable.jpg" width="300"/> <img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/cosse.jpg" width="300"/>


### Relier un câble USB au ventillo

> [!NOTE]
> Ce câble fera le lien entre le ventilateur et la raspberry. Brancher le ventilateur sur la carte pemet de l'alimenter et de le faire fonctionner.

- couper le câble USB à une trentaine de centimètre du branchement USB  
- enfiler la gaine thermo sur le câble (elle sera chauffée à la fin)   
- souder les câbles rouges ensemble et les câbles noirs ensemble  

<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/ventilateur_cable.jpg"  width="300"/>

### Relier des câbles de prototypage au bouton poussoir  

> [!NOTE]
> Ces câbles feront le lien entre le bouton poussoir et la raspberry.

- répéter les mêmes étapes que pour le câble USB et le ventillo  

<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/bp_cable.jpg" width="300"/>

### Etape 2 - assemblage de la carte ethernet et de la carte raspberry  

> [!NOTE]
> La carte Ethernet est nécessaire pour ""

- monter les supports sur la raspberry
- souder barette noire
- brancher carte ethernet sur raspberry
- connecter les "trames"

<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/support_raspberry.jpg" width="300"/> <img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/ethernet_raspberry.jpg" width="300"/> <img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/trame_ethernet.jpg" width="300"/>

### Etape 3 - Perçage des côtés du boitier 

> [!NOTE]
> Ces ouvertures permettront de placer les connecteurs.

> [!TIP]
> Réaliser une ouverture supplémentaire pour que l'air puisse circuler et refroidir le système
>
> Si votre boitier est différent réfléchisser à la meilleur manière de l'organiser à l'intérieur

- percer des trous pour les connecteurs et leurs vis
  - (1) connecteur HDMI femelle/femelle : un trou de 22mm de diamètre et 2 trous de 3.5mm (vis)
  - (2) connecteur ethernet femelle/femelle : un trou de 27mm de diamètre
  - (3) bouton poussoir : un trou de 16mm de diamètre
  - (4) commutateur : un trou de 29mm * 22mm
  - (5) ventillateur : un trou de 26mm de diamètre et 4 trous de 3mm (vis)
  - (6) aération : un trou de 20mm de diamètre
  - (7) fixation raspberry au boitier : 4 trous de 2.5mm (vis)
  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/1d26dc7c550473cd11c55e5427cf5d3865ed02c2/docs/pictures/assembly_guide/boitier/boitier_trou.jpg" width="300"/>

### Etape 4 - Fixation du receiver gaming, de la carte gps et du ventilateur dans le boitier

- fixer le receiver gaming et la carte gp à l'aide de velcro
- visser le ventilateur
- brancher le câble micro USB sur la carte gps, il sera difficile d'accès lorsque la carte raspberry sera fixée
  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/gps_receiver_ventilateur.jpg" width="300"/>

 ### Etape 5 - Fixation du clavier et de la batterie dans le couvercle  
 - fixer le clavier et la baatterie à l'aide de velcro
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/fixer_batterie_clavier.jpg" width="300"/>

### Etape 6 - Fixation de la raspberry au boitier

<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/d7f3a26780ae5b1e7ddae37c8ff18bae6e9926e9/docs/pictures/assembly_guide/branchement_gps_gaming.jpg" width="300"/>

### Etape 7 - Fixation de l'interrupteur, du bouton poussoir, des connecteurs et réalisation des branchements

![cablage final](pictures/assembly_guide/boitier/cablage_final_v2.jpg)

## 2. Assemblage du caisson vidéo
<details>
  <summary> Outils </summary>
  
  * ex1
  * ex2
  
</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel caisson vidéo](/../µKOSMOS/hardware/04_materiel_caisson_video.md)
    
</details>

## 3. Assemblage du trépried
<details>
  <summary> Outils </summary>
  
  * imprimante 3D {[Etape 1](assemblage_µkosmos.md#etape-1---impression-3d)}
  * foret M3, M6 {[Etape 2](assemblage_µkosmos.md#etape-2---assemblage-de-la-partie-inf%C3%A9rieur-du-tr%C3%A9pied)}
  * meuleuse {[Etape 2](assemblage_µkosmos.md#etape-2---assemblage-de-la-partie-inf%C3%A9rieur-du-tr%C3%A9pied)}

</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel trépied](/../µKOSMOS/hardware/07_materiel_trepied.md)
    
</details>

### Etape 1 - Impression 3D
Imprimer les pièces inférieur et supérieur du socle ainsi que les pièces de maintient du caisson vidéo.

### Etape 2 - Assemblage de la partie inférieur du trépied
 - Découper le tube en aluminium de manière à obtenir trois segments d'environ "500mm". Ces segments formeront les trois pieds.
 - Couper les extrémitées de chaque segment en biais (environ 45°). Cela permet de les poser à plat tout en étant inclinés et de prendre moins de place sous les support du caisson vidéo.
 - Percer les tubes avec un foret de 6mm à environ 20cm du bord (un peu plus que la longueur des plombs que vous avez choisis). Ceci est la partie basse des pieds
 - Percer deux trous àl'autre extrémité du tube. Un avec un foret de 3mm à environ 20mm du bord du tube et un autre à 100mm du bord. Les trous doivent traversés le tube de part et d'autre pour pouvoir y insérer des vis.
 - Percer les plombs avec un foret de 3mm perpendiculairement au trou déjà existant. Ce trou permettra de faire passer le serre câble pour maintenir la partie basse du plomb sur le tube.
 - Fixer les plombs sur la partie basse des pieds. Visser et ajouter un serre câble comme ci-dessous.
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/fixation_plomb.jpg" width="300"/>  

 - Couper le tête des clous, insérer les dans les trou réalisés à 100mm de la partie haute et plier les bords qui dépasse contre le tube. Ces clous servent de butée et empèche la partie inférieur du socle de glisser plus bas.  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/positionnement_clou.jpg" width="300"/>

 - Insérer la partie haute des tubes dans le socle inférieur du trépied imprimée en 3D  
 - Faire passer un fil de fer dans les trous réalisés à 20mm de la partie haut. Ce fil sert de butée et empèche la partie inférieur du socle de glisser vers le haut.     
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/montage_fil.jpg" width="300"/>
  
### Etape 3 - Assemblage de la partie supérieur du trépied
 - Coller les bandes de mousse à l'intérieur des bers. Attention à laisser les trous prévus pour les vis libres.
 - Percer 2 trous dnas la plaque métalique avec un foret M4 et un trou avec un foret M10. Il faut que les trous correspond aux trous déjà présent sur la partie centrale du socle supérieur imprimé en 3D
 - Positionner la plaque métallique au dessus de la partie supérieur du socle et fixer l'anneau d'accroche M10 à la partie supérieur du socle.  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/fixation_anneau.jpg" width="300"/>

 - Visser le ber supérieur à la partie supérieur du socle avec des vis M4  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/fixation_ber.jpg" width="300"/>

 - Visser le "ber inférieur" pour former le support du caisson vidéo. (Pas besoin de serrer pour le moment si vous n'avez pas inséré le caisson.)

### Etape 4 - Assemblage de la partie haute et de la partie basse du trépied
 - Découper la tige filetée de manière à avoir 2 segments de 170mm et 4 segements de 145mm
 - inserrer des écrous nylstop de chaque côté des tiges filetées  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/positionnement_nylstop.jpg" width="300"/>

 - Lors du montage des écrous placer des rondelles de chaque côté de la pièce imprimer pour la protéger. Insérer les tiges filetée dans le socle inférieur puis Visser un écrou avec oreilles en dessous.  
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/46f831fdac85ba5268682a896dfe86de68dc4d20/docs/pictures/assembly_guide/trepied/positionnement_rondelle_ecrou.jpg" width="300"/>

 - Insérer des rondelles sur les tiges puis positionner la partie supérieur du socle. Ajuster les écrous de manière à ce que le socle vienne se poser horizontallement.
 - Comme pour la partie basse fixer le haut avec des écrous à oreilles
   
   ![imagefinale](pictures/assembly_guide/trepied/final_v2.png)
   
## 4. Assemblage du casque
<details>
  <summary> Outils </summary>
  
  * foret M2 {[Etape 3](assemblage_µkosmos.md#etape-3---percer-la-coque-ext%C3%A9rieur-du-casque)}
  
</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel casque](/../µKOSMOS/hardware/05_materiel_casque.md)
    
</details>

### Etape 1 - Impression 3D
Imprimer les pièces de suport de l'écran ainsi que celles du support de batterie.

### Etape 2 - Assemblage écran
 - Visser l'écran à sont support
 - Mettre de la mousse sur les diagonales du support d'écan
 - brancher un cable micro usb
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/2b400d2080259c5bb73a4db916ddbb828bc9c9a8/docs/pictures/assembly_guide/casque/support_ecran.jpg" width="300"/>

### Etape 3 - Percer la coque extérieur du casque
 - Réaliser une ouverture sur le haut du casque pour pouvoir accéder à la prise hdmi de l'écran
 - Percer également l'avant de la coque pour pouvoir visser la partie basse du support de la batterie.
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/fefa367d9d9f9491e3bdaf13d451372837209f19/docs/pictures/assembly_guide/casque/trou_coque.jpg" width="300"/>

### Etape 4 - Assemblage de la batterie

> [!NOTE]
> Sur les supports la mousse permet de caler les éléments.

 - Mettre de la mousse sur les diagonales du support inférieur et supérieur de la batterie
   
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/2b400d2080259c5bb73a4db916ddbb828bc9c9a8/docs/pictures/assembly_guide/casque/bot_support.jpg" width="300"/> <img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/2b400d2080259c5bb73a4db916ddbb828bc9c9a8/docs/pictures/assembly_guide/casque/top_support_bat.jpg" width="300"/> 

 - Visser la partie basse du support de la batterie au casque
 - placer la batterie à l'intérieur
 - visser la partie supérieur du supporrt pour le fermer

### Etape 5 - Asssemblage final
 - Mettre l'écran dans le casque
 - fermer le casque
 - brancher le cable hdmi et relier le cable usb à la batterie
<img src="https://github.com/Hclothilde/Documentation_KOSMOS/blob/2b400d2080259c5bb73a4db916ddbb828bc9c9a8/docs/pictures/assembly_guide/casque/casque_entier.jpg" width="800"/>

## 5. Assemblage du câble
<details>
  <summary> Outils </summary>
  
  * ex1
  * ex2
  
</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel câble](/../µKOSMOS/hardware/03_materiel_cable.md)
    
</details>

## 6. Assemblage de la paravane
<details>
  <summary> Outils </summary>
  
  * ex1
  * ex2
  
</details>

<details>
  <summary> Materiel </summary>
  
  [Tableau matériel paravane](/../µKOSMOS/hardware/06_materiel_paravane.md)
    
</details>



    
