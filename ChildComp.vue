<script setup>
// TODO 2 — Déclarer la prop 'msg' (type String) avec defineProps()


// TODO 3 — Déclarer l'événement 'reponse' avec defineEmits()

</script>

<template>
  <div class="child">
    <!-- 1. Composant de base -->
    <p>Je suis le composant enfant !</p>

    <!-- TODO 2 — Afficher la prop msg (avec v-if) -->

    <!-- TODO 3 — Ajouter un bouton qui émet 'reponse' au clic -->

    <!-- TODO 4 — Ajouter un <slot /> pour le contenu du parent -->
  </div>
</template>

<style scoped>
.child {
  border: 2px solid #42b883;
  padding: 14px 18px;
  border-radius: 10px;
  background: white;
  box-shadow: 0 2px 8px rgba(66, 184, 131, 0.15);
}

.child p {
  margin: 0;
  color: #35495e;
}

.prop {
  margin-top: 8px !important;
  color: #2980b9 !important;
  font-style: italic;
}

button {
  margin-top: 10px;
  padding: 6px 14px;
  background: #42b883;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-size: 0.9em;
}

button:hover {
  background: #38a373;
}
</style>
