<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

// TODO 2 — Créer une ref 'message' avec le texte 'Salut depuis le parent !'


// TODO 3 — Créer une ref 'messageEnfant' avec 'En attente...'

</script>

<template>
  <div class="app">
    <h1>Démo Composants Vue.js</h1>

    <!-- 1. Composant (déjà fait !) -->
    <section>
      <h2>1. Composant</h2>
      <ChildComp />
    </section>

    <!-- 2. Props -->
    <section>
      <h2>2. Props</h2>
      <!-- TODO 2 — Passer la prop :msg="message" à ChildComp -->
      <ChildComp />
    </section>

    <!-- 3. Emits -->
    <section>
      <h2>3. Emits</h2>
      <!-- TODO 3 — Afficher messageEnfant et écouter @reponse sur ChildComp -->
      <ChildComp />
    </section>

    <!-- 4. Slots -->
    <section>
      <h2>4. Slots</h2>
      <!-- TODO 4 — Injecter du contenu HTML entre les balises de ChildComp -->
      <ChildComp />
    </section>
  </div>
</template>

<style scoped>
.app {
  max-width: 600px;
  margin: 0 auto;
  font-family: system-ui, sans-serif;
  color: #2c3e50;
}

h1 {
  color: #42b883;
  border-bottom: 3px solid #42b883;
  padding-bottom: 8px;
}

h2 {
  color: #35495e;
  font-size: 1.2em;
}

section {
  margin: 20px 0;
  padding: 16px;
  background: #f8fafb;
  border-radius: 10px;
}

.received {
  color: #e67e22;
  font-weight: bold;
}
</style>
