# Bataille des artisans v1: Le mini zillo-mini-devkit !

Salut les bagarreurs!

Vous avez recu votre colis? Vous vous demandez ce que c'est ? Si ca va exploser ? Nous tenterons ici de repondre a (presque) toutes vos questions!

## Contenu du colis

- Un "zillo-mini-devkit"

(image)

- Des stickers

- Un trophée (si vous avez été sage)

(image)

## Le zillo-mini-devkit c'est quoi???

C'est une plateforme d'immagination et de developpement pour la Bataille-des-artisans

Son hardware est le suivant:

### ESP32-WROOM

(image)

L'ESP32 est un module 'tout en un' comprenant de nombreuses fonctionnalités.
C'est un microcontroleur 32bit multi-coeur cadence a xx mhz.
Il dispose nativement de fonctionnalités WIFI, de ports série, d'un systeme de fichiers minimaliste et d'une memoire flash de 4mo, permettant de stocker programme et assets.
(liste de fonctionnalités non exhaustive)

Il est programmable via son port USB avec un framework Arduino.

Plus d'explications l'ESP32. avec des docs, a venir !

![esp32 pinout](doc/ESP32-Pinout.png)

### Matrice de leds WS2812b

(image)

C'est une matrice de leds RGB adressables (c'est a dire qu'elle sont controlables individuellement), qui utilise un bus de communication entre les leds pour passer le signal de led en led.

Des librairies permettront le pilotage de ces leds sans se preocupper de leur protocole de communication.

Plus d'infos sur les leds WS2812b communement appeles "NEOPIXELS", et leur matrices  sur le internet par ici:

(liens adafruit)

### MPU6050

(image)

Le module MPU6050 est une puce tout-en-un qui contient 3 accelerometres et 3 gyroscopes.
Il permet ainsi d'obtenir des informations concernant l'acceleration et l'orientation de l'objet.

La communication entre le programme et le MPU6050 s'effectue via le protocole I2C.

Des librairies permettront l'interrogation facile de toutes ces valeurs.

(lien datasheet)

### Micro+MAX4466

(image)

Le micro est relie a une entree analogique de l'ESP32 et permet par exemple de detecter le niveau de bruit ambiant.

Il ne sera malheureusement pas assez precis pour des usages plus aboutis, de maniere simple, dans notre projet.

Cependant Fourrier, et ses transformations, est peut-etre notre ami! (ou pas)

(lien datasheet)

### Buzzer disque

(images)

Le buzzer est relié directement a une sortie PWM de l'ESP32. Le PWM permet de moduler la frequence d'un signal, ce qui a pour effet de produire des tonalités ou melodies lorsque connecté a un haut parleur basique.

Dans notre projet il n'y a malheureusement pas de circuit d'amplification du signal, ni de haut parleur assez puissant permettant de faire un son "fort"

### Un circuit imprimé (PCB) permettant de connecter le tout

(images)

//todo: refaire image

![front](https://i.imgur.com/w5FB8dj.png)
![back](https://i.imgur.com/TXoOl5r.png)

### boitier

//todo: refaire image

![defaut](https://i.imgur.com/voREZIB.png)
