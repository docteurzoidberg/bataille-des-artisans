<template>
  <Page title="Bataille des artisans: Le zillo-mini-devkit !" icon="mdi-gift">

    <p>Salut les bagarreurs!</p>

    <p>Vous avez recu votre colis ? Vous vous demandez ce que c'est ? Si ça va exploser ? Nous tenterons ici de répondre à (presque) toutes vos questions!</p>

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
      Le zillo-mini-devkit c'est quoi ???
    </h2>

    <p>C'est une plateforme d'imagination et de développement pour la Bataille-des-artisans</p>

    <p>Son hardware est le suivant :</p>

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
          lazy="false"
        >
          <template v-slot:placeholder>
            <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
            >
              <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
        <v-card-text class="text--primary">
          Board ESP32
        </v-card-text>
      </v-card>
    </p>
    <p>
      L'ESP32 est un module 'tout en un' comprenant de nombreuses fonctionnalités.
      Il a plusieurs coeurs, dispose nativement de fonctionnalités WIFI, de ports série, d'un système de fichiers minimaliste et d'une mémoire flash de 4 Mo, permettant de stocker programme et assets.
      (liste de fonctionnalités non exhaustive)
    </p>

    <p>Il est programmable via son port USB avec un framework Arduino.</p>

    <p>Plus d'explications techniques sur l'ESP32 ici: <a href="https://fr.wikipedia.org/wiki/ESP32" target="_blank">https://fr.wikipedia.org/wiki/ESP32</a></p>

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
        />
        <v-card-text class="text--primary">
          Matrice 8x8 WS2812b
        </v-card-text>
      </v-card>
    </p>

    <p>C'est une matrice de leds RGB adressables (c'est a dire qu'elles sont controlables individuellement), qui utilise un bus de communication entre les leds pour passer le signal de led en led.</p>

    <p>Des librairies permettront le pilotage de ces leds sans se préocupper de leur protocole de communication.</p>

    <p>Plus d'infos sur les leds WS2812b communément appelées "NEOPIXELS", et leur matrices  sur internet par ici : <a href="https://learn.adafruit.com/adafruit-neopixel-uberguide/" target="blank">https://learn.adafruit.com/adafruit-neopixel-uberguide/</a></p>

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
        />
        <v-card-text class="text--primary">
          Board MPU6050
        </v-card-text>
      </v-card>
    </p>

    <p>
      Le module MPU6050 est une puce tout-en-un qui contient 3 accéléromètres et 3 gyroscopes.
      Il permet ainsi d'obtenir des informations concernant l'accélération et l'orientation de l'objet.
    </p>

    <p>La communication entre le programme et le MPU6050 s'effectue via le protocole I2C.</p>

    <p>Des librairies permettront l'interrogation facile de toutes ces valeurs.</p>

    <p>(lien vers la doc à venir)</p>

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
        />
        <v-card-text class="text--primary">
          Board Micro + MAX4466
        </v-card-text>
      </v-card>
    </p>

    <p>Le micro est relié à une entrée analogique de l'ESP32 et permet par exemple de détecter le niveau de bruit ambiant.</p>

    <p>Il ne sera malheureusement pas assez précis pour des usages plus aboutis, de manière simple, dans notre projet.</p>

    <p>Cependant Fourrier, et ses transformations, est peut-être notre ami! (ou pas)</p>

    <p>(lien vers la doc à venir)</p>

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
        />
        <v-card-text class="text--primary">
          Speaker piezzo-electrique
        </v-card-text>
      </v-card>
    </p>

    <p>Le buzzer est relié directement à une sortie PWM de l'ESP32. Le PWM permet de moduler la fréquence d'un signal, ce qui a pour effet de produire des tonalités ou mélodies lorsque connecté à un haut parleur basique.</p>

    <p>Dans notre projet il n'y a malheureusement pas de circuit d'amplification du signal, ni de haut parleur assez puissant permettant de faire un son "fort".</p>

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
          >
          <template v-slot:placeholder>
            <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
            >
              <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
        <v-card-text class="text--primary">
          PCB custom
        </v-card-text>
      </v-card>
    </p>

    <h3 id="uncircuitimprimpcbpermettantdeconnecterletout">
      Dans un boitier et son diffuseur lumineux imprimés en 3D
    </h3>

    <p>
      <v-card outlined>
        <v-img
          height="450"
          src="https://i.imgur.com/p7HiKHi.png"
          alt="pcb"
          contain
          aspect-ratio
          >
          <template v-slot:placeholder>
            <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
            >
              <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
        <v-card-text class="text--primary">
          Boitier 3D sous OpenScad
        </v-card-text>
      </v-card>
    </p>
  </Page>
</template>

<script>
import Page from '~/components/Page.vue'
export default {
  components: {
    Page
  }
}
</script>
