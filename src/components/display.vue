<template>
  <div class="conteneur">
    <div class="display">
      <p>{{ count }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "display",
  props: {
    count: Number,
  },
};
</script>

<style>
.display {
  display: flex;
  justify-content: center;
  align-items: center;
  color: #ecf39e;
  background-color: #4f772d;
  border: 5px solid #132a13;
  width: 20vh;
  height: 10vh;
}
.display p {
  font-family: "Alfa Slab One", cursive;
  font-size: 50px;
  color: #ecf39e;
}
</style>