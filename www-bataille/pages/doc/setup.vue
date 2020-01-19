<template>
  <Page title="Setup son environnement de developpement" icon="mdi-tools">

    <h2>Pre-requis</h2>

    <h3>Logiciels a avoir</h3>

    <h4>
      Visual Studio Code
      <a href="https://code.visualstudio.com/download" target="_blank">(lien)</a>
    </h4>
    <p>On ne vous le présente plus !</p>

    <h4>
      PIO (extension vscode)
      <a href="https://platformio.org/install/ide?install=vscode" target="_blank">(lien)</a>
    </h4>
    <p>
      Extension permettant l'integration de multiples frameworks IOT au sein de vscode.<br/>
      PIO gerera pour vous l'installation du framework arduino, des librairies, de compiler le code, de flasher l'esp32 (etc), d'ouvrir le moniteur serie (entre autres)
    </p>

    <h4>
      OpenScad
      <a href="https://www.openscad.org/downloads.html" target="_blank">(lien)</a>
    </h4>
    <p>
      Logiciel de 3d parametrique.<br/>
      Vous permetra d'editer les sources du boitier et du diffuseur.
    </p>

    <h4>
      KiCad (facultatif)
      <a href=" https://kicad-pcb.org/download/" target="_blank">(lien)</a>
    </h4>
    <p>
      Outil "EDA" de conception de circuits electroniques.<br/>
      Vous permetra de consulter les sources du schéma electronique et du circuit imprimé.
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
