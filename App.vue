<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

// 1 — Props : donnée à passer à l'enfant
const greeting = ref('Hello du parent')

// 2 — Emits : message reçu de l'enfant
const childMsg = ref('Pas encore de message')
</script>

<template>
  <h2>Composants Vue.js</h2>

  <!-- 1 — Props : passer greeting comme prop msg -->
  <ChildComp :msg="greeting" @response="(msg) => childMsg = msg">
    <!-- 3 — Slots : contenu injecté dans le slot de l'enfant -->
    <em>Contenu injecté depuis le parent !</em>
  </ChildComp>

  <!-- 2 — Emits : afficher le message reçu de l'enfant -->
  <p>{{ childMsg }}</p>
</template>
