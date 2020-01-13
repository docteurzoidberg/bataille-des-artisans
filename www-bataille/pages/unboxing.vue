<template>
  <v-layout>
    <v-flex id="playground-example" class="overflow-y-auto">
      <v-card>
        <v-card-title>
          <h1 class="accent--text" id="batailledesartisansv1leminizillominidevkit">
            Bataille des artisans v1: Le zillo-mini-devkit !
          </h1>
        </v-card-title>
        <v-card-text class="text-left">
          <p>Salut les bagarreurs!</p>

          <p>Vous avez recu votre colis? Vous vous demandez ce que c'est ? Si ca va exploser ? Nous tenterons ici de repondre a (presque) toutes vos questions!</p>

          <h2 id="contenuducolis">
            Contenu du colis
          </h2>

          <ul>
            <li><p>Un "zillo-mini-devkit"</p></li>

            <li><p>Des stickers</p></li>

            <li><p>Un trophée (si vous avez été sage)</p></li>
          </ul>

          <p>(image)</p>

          <h2 id="lezillominidevkitcestquoi">
            Le zillo-mini-devkit c'est quoi???
          </h2>

          <p>C'est une plateforme d'immagination et de developpement pour la Bataille-des-artisans</p>

          <p>Son hardware est le suivant:</p>

          <h3 id="esp32wroom">
            ESP32-WROOM
          </h3>
          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/ESP32-DevKitC.png"
                alt="esp32"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
                Board ESP32
              </v-card-text>
            </v-card>
          </p>
          <p>
            L'ESP32 est un module 'tout en un' comprenant de nombreuses fonctionnalités.
            C'est un microcontroleur 32bit multi-coeur cadence a xx mhz.
            Il dispose nativement de fonctionnalités WIFI, de ports série, d'un systeme de fichiers minimaliste et d'une memoire flash de 4mo, permettant de stocker programme et assets.
            (liste de fonctionnalités non exhaustive)
          </p>

          <p>Il est programmable via son port USB avec un framework Arduino.</p>

          <p>Plus d'explications l'ESP32. avec des docs, a venir !</p>

          <h3 id="matricedeledsws2812b">
            Matrice de leds WS2812b
          </h3>

          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/ledmatrix.jpg"
                alt="ledmatrix"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
               Matrice 8x8 WS2812b
              </v-card-text>
            </v-card>
          </p>

          <p>C'est une matrice de leds RGB adressables (c'est a dire qu'elle sont controlables individuellement), qui utilise un bus de communication entre les leds pour passer le signal de led en led.</p>

          <p>Des librairies permettront le pilotage de ces leds sans se preocupper de leur protocole de communication.</p>

          <p>Plus d'infos sur les leds WS2812b communement appeles "NEOPIXELS", et leur matrices  sur le internet par ici:</p>

          <p>(liens vers la doc adafruit a venir)</p>

          <h3 id="mpu6050">
            MPU6050
          </h3>

          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/mpu6050.jpg"
                alt="mpu6050"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
               Board MPU6050
              </v-card-text>
            </v-card>
          </p>

          <p>
            Le module MPU6050 est une puce tout-en-un qui contient 3 accelerometres et 3 gyroscopes.
            Il permet ainsi d'obtenir des informations concernant l'acceleration et l'orientation de l'objet.
          </p>

          <p>La communication entre le programme et le MPU6050 s'effectue via le protocole I2C.</p>

          <p>Des librairies permettront l'interrogation facile de toutes ces valeurs.</p>

          <p>(lien vers la doc a venir)</p>

          <h3 id="micromax4466">
            Micro+MAX4466
          </h3>

          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/max4466.jpg"
                alt="max4466"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
               Board Micro + MAX4466
              </v-card-text>
            </v-card>
          </p>

          <p>Le micro est relie a une entree analogique de l'ESP32 et permet par exemple de detecter le niveau de bruit ambiant.</p>

          <p>Il ne sera malheureusement pas assez precis pour des usages plus aboutis, de maniere simple, dans notre projet.</p>

          <p>Cependant Fourrier, et ses transformations, est peut-etre notre ami! (ou pas)</p>

          <p>(lien vers la doc a venir)</p>

          <h3 id="buzzerdisque">
            Buzzer disque
          </h3>

          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/piezzospkr.jpg"
                alt="speaker"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
               Speaker piezzo-electrique
              </v-card-text>
            </v-card>
          </p>

          <p>Le buzzer est relié directement a une sortie PWM de l'ESP32. Le PWM permet de moduler la frequence d'un signal, ce qui a pour effet de produire des tonalités ou melodies lorsque connecté a un haut parleur basique.</p>

          <p>Dans notre projet il n'y a malheureusement pas de circuit d'amplification du signal, ni de haut parleur assez puissant permettant de faire un son "fort"</p>

          <h3 id="uncircuitimprimpcbpermettantdeconnecterletout">
            Un circuit imprimé (PCB) permettant de connecter le tout
          </h3>

          <p>
            <v-card outlined>
              <v-img
                height="350"
                src="/pictures/pcb.jpg"
                alt="pcb"
                contain
                aspect-ratio
              ></v-img>
              <v-card-text class="text--primary">
               PCB custom
              </v-card-text>
            </v-card>
          </p>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>
