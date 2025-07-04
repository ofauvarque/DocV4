# **Assemblage de la batterie**

Nous avons choisi de concevoir nous-mêmes la batterie de notre système, ce qui nous permet d'obtenir une solution durable et économique.

### **Éléments nécessaires**

#### **Outils**

##### - **En général**

<img src="../../pictures/02_Batterie/wire_stripper.jpg" alt="Wire Stripper" height="300"> <img src="../../pictures/02_Batterie/soldering_iron.jpg" alt="Fer à Souder" height="300"> <img src="../../pictures/02_Batterie/tin.jpg" alt="Bobine étain" height="300">

- **Pince à dénuder :** Réglable, comme sur l'image, pour différents types de câbles.
- **Fer à souder**
- **Bobine d'étain**
- **Source de chaleur pour gaine thermorétractable :** Un pistolet à air chaud, un chalumeau ou un fer à souder

##### - **Pour la soudure des accumulateurs**

<img src="../../pictures/02_Batterie/lithium_acu_soldering_equipment.jpg" alt="Equipement Soudure Acu" width="400">

- **Gants de protection**
- **Lunettes de protection**
- **Pince à couper :** Pour découper les bandes de nickel.
- **Ruban adhésif :** Utilisé temporairement pour maintenir en place différents composants.
- **Soudeuse par points**
- **Seau de sable :** Pour étouffer un éventuel début de flamme des accumulateurs.

#### **Composants**

<img src="../../pictures/02_Batterie/components_overview.jpg" alt="Components Overview" width="600">

- **Deux câbles d'alimentation :** Ces câbles servent à la charge et à la décharge de la batterie. Le courant en sortie de la batterie n'étant pas très élevé, quelques ampères, pas besoin d'une grande section de câbles.
- **Connecteurs XT30 mâle et femelle**
- **Gaines thermorétractables**
- **9 accumulateurs lithium-ion**
- **BMS**
- **4 câbles :** Reliant le BMS aux accumulateurs, de préférence de couleurs distinctes pour une identification facile.
- **Plaque de nickel en ruban**
- **Ruban adhésif kapton**

### **⚠️ Attention:**

**À cette étape de la conception de notre système, certaines parties présentent des risques. Il est donc essentiel de rester vigilant et de respecter scrupuleusement les mesures de protection recommandées.**

## **1. Vue d'ensemble de la partie batterie**

La batterie se compose des 9 accumulateurs connectés au module BMS selon un schéma spécifique. Le seul connecteur externe est un XT30, utilisé à la fois pour la charge et la décharge.

|<img src="../../pictures/02_Batterie/schema_bms.png" alt="Acus Soudés par 3 avec 4 bandes" width="330">|
|:--:|
|*Schéma de branchement*|

### **1.1 Connecteur XT30**

---

<img src="../../pictures/02_Batterie/xt30_soldered.jpg" alt="Deux Câbles avec XT30" width="250">

Les deux câbles d'alimentation doivent être légerement étamés puis soudés sur le connecteur XT30 femelle, en respectant les couleurs et les signes, le rouge sur le **+** et le noir sur le **-**. Ne pas oublier les gaines thermorétractables, à chauffer avec un décapeur thermique, briquet ou fer à souder, attention cependant à ne pas l'abîmer en chauffant trop.

---

Après avoir préparé le connecteur XT30, il faut maintenant raccorder les deux câbles au module BMS.

Commencez par dénuder légèrement les extrémités des câbles.

**⚠️ Attention à ne pas trop dénuder : une trop grande longueur de fil nu augmente le risque de contact entre les deux pôles, ce qui pourrait provoquer un court-circuit.**

<img src="../../pictures/02_Batterie/bms_power_cables.jpg" alt="Deux Câbles Prêts à être Soudés sur BMS" width="250">

Comme pour le connecteur XT30, attention à bien respecter le signe pour chaque câble.

### **1.2 Assemblage des Accumulateurs et BMS**

---

Avant de commencer, assurez-vous que la soudeuse par points est bien chargée et opérationnelle.

|<img src="../../pictures/02_Batterie/bms_on_battery.jpg" alt="Vue de la Batterie Finie" width="300">|
|:--:|
| *Résultat à la fin de l'assemblage (avec un autre type de câbles)* |

**⚠️ Attention: Les accumulateurs lithium-ion sont sensibles à la manipulation. Un court-circuit peut provoquer un départ de feu. Il est donc essentiel de réduire les risques au maximum.**

---

#### Préparation de la zone de travail

Avant toute opération, sécurisez l'environnement :

- Éloignez tout produit inflammable.
- Préparez un seau de sable à portée de main (en cas d'incident).
- Équipez-vous de gants et de lunettes de protection.

---

#### Assemblage des accumulateurs

- Formez trois groupes de trois accumulateurs. Chaque groupe représente une chaîne de trois accumulateurs en parallèle, ce qui est un modèle 3S3P (3 en série et 3 en parallèle).
- Chaque groupe est constitué de trois accumulateurs alignés dans le même sens : le pôle positif (bombé) d'un côté, et le pôle négatif (plat) de l'autre.
- Disposez chaque groupe en quinconce, comme montré sur l'image ci-dessous.

<img src="../../pictures/02_Batterie/lithium_acu_before_soldering.jpg" alt="Acus Prêts à être soudés par 3" width="400">

- Utilisez du ruban adhésif pour maintenir temporairement chaque groupe en place. Cela facilite la soudure et évite les mouvements indésirables.
- Découpez une bande de nickel pour chaque groupe afin de relier les trois pôles entre eux.

<img src="../../pictures/02_Batterie/lithium_acu_nickel_plate.jpg" alt="Acus Prêts à être soudés par 3" width="300">

---

#### Soudure par points

- Soudez les bandes de nickel en appliquant quatre points de soudure par pôle, en formant un motif en diagonale pour une bonne répartition.

<img src="../../pictures/02_Batterie/lithium_acu_nickel_plate_soldered_colored.jpg" alt="Acus Soudés par 3" width="300">

- Répétez cette opération jusqu'à ce que chaque pôle de chaque groupe soit correctement connecté à sa bande de nickel. Cela nécessite 6 bandes en tout (3 groupes avec 2 côtés).

---

#### Assemblage final des blocs

Vous avez maintenant trois blocs de trois accumulateurs chacun. Avant de les assembler entre eux, il est nécessaire d'inverser l'orientation du bloc central, c'est essentiel pour respecter le schéma de connexion en série, où les pôles opposés se connectent entre eux (le + d'un bloc vers le - du bloc suivant), tout en respectant la configuration 3S3P.

- Découpez 4 bandes supplémentaires de nickel pour relier les blocs entre eux, selon le schéma.

<img src="../../pictures/02_Batterie/schema_bms.png" alt="Acus Soudés par 3 avec 4 bandes" width="400">

- Rappel : le pôle positif est le côté bombé, et le pôle négatif est le côté plat.

Enfin, vous obtiendrez un ensemble de blocs soudés comme ci-dessous. Les couleurs correspondent aux futures connexions du BMS.

<img src="../../pictures/02_Batterie/lithium_acu_nickel_plates_soldered_colored.jpg" alt="Acus Soudés Face 1" width="300">

---

#### Connexion entre le BMS et les accumulateurs

Une fois les blocs soudés entre eux, on peut passer à l'étape du câblage entre le BMS et les accumulateurs.

Pour cela, vous aurez besoin de :

- 4 câbles (de couleurs différentes, comme sur le schéma)
- 4 petits carrés de plaque de nickel

<img src="../../pictures/02_Batterie/four_cables_and_four_squares_of_nickel.jpg" alt="4 câbles avec plaques de nickel" width="300">

Commencez par souder chaque câble sur un carré de nickel, à l'étain.

<img src="../../pictures/02_Batterie/four_cables_soldered_on_nickel.jpg" alt="4 câbles soudés sur plaques de nickel" width="300">

---

#### Détermination de la longueur des câbles

Pour déterminer la longueur idéale des câbles, fixez temporairement le BMS sur le côté des accumulateurs avec un morceau de ruban adhésif. Cela vous permet de positionner les câbles avec précision.

Ensuite :

- Repérez et marquez la bonne longueur.
- Coupez les câbles en conséquence.
- Dénudez-les légèrement.
- Soudez-les sur les bornes du BMS, en respectant les couleurs et l'ordre indiqués dans le schéma de câblage.

<img src="../../pictures/02_Batterie/four_cables_soldered_on_nickel_right_length.jpg" alt="4 câbles soudés et coupés à la bonne longueur" height="250"> <img src="../../pictures/02_Batterie/four_cables_soldered_on_bms.jpg" alt="4 câbles soudés sur BMS" height="250">

---

#### Connexion finale à la batterie

Il est temps de souder les extrémités libres des câbles sur les zones correspondantes des accumulateurs. Encore une fois, vous pouvez fixer temporairement le BMS avec du ruban pour faciliter le positionnement.

<img src="../../pictures/02_Batterie/red_blue_soldered_on_battery.jpg" alt="câble rouge et bleu sur BMS" height="300"> <img src="../../pictures/02_Batterie/yellow_black_soldered_on_battery.jpg" alt="câble jaune et noir sur BMS" height="300">

---

#### Vérification du montage

Avant de finaliser, prenez un multimètre et mesurez la tension entre les bornes + et - de la batterie. Si vous lisez une tension cohérente (autour de 10-12V selon l'état de charge), c'est que tout est correctement câblé.

---

#### Finition

Retirez le ruban temporaire et enveloppez l'ensemble de la batterie avec du ruban adhésif kapton pour la protéger et maintenir l'assemblage.

<img src="../../pictures/02_Batterie/battery_covered.jpg" alt="batterie couverte kapton" height="350">