<template>
<div class="tt2">
  <input type="submit" v-on:click="$emit('validation')" value="save and continue"> <!-- ici j'ai réalisé cela avec un v-on click mais il faudrait utiliser un v-on submit ou alors creer un method {} pour ensuite mettre un onsubmit -->
</div> <!-- ainsi au lieu que le message s'affiche au clique il s'afficherait lors du submit des réponse et serait donc bloqué avec les required -->
</template>

<script>
export default {
  name: "Button",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>