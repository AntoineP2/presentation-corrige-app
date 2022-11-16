<template>
  <div class="conteneur">
    <button class="buttonCount" @click="$emit('increment')">
      <p>Incrémenter</p>
    </button>
  </div>
</template>

<script>
export default {
  name: "buttonCount",
};
</script>

<style>
</style>