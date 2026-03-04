<script setup>
// 1 — Props : déclarer la prop msg reçue du parent
defineProps({
  msg: String
})

// 2 — Emits : déclarer et émettre l'événement response
const emit = defineEmits(['response'])
emit('response', "hello de l'enfant")
</script>

<template>
  <!-- 1 — Props : afficher la prop msg -->
  <p>{{ msg }}</p>

  <!-- 3 — Slots : emplacement pour le contenu du parent -->
  <slot>Contenu de secours</slot>
</template>
