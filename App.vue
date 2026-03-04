<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

// TODO 1 — Props : créer une ref 'greeting' avec le texte 'Hello du parent'


// TODO 2 — Emits : créer une ref 'childMsg' avec 'Pas encore de message'

</script>

<template>
  <h2>Composants Vue.js</h2>

  <!-- TODO 1 — Props : passer la prop :msg="greeting" à ChildComp -->
  <ChildComp />

  <!-- TODO 2 — Emits : écouter @response sur ChildComp et afficher childMsg -->

  <!-- TODO 3 — Slots : utiliser ChildComp avec du contenu entre les balises -->
</template>
