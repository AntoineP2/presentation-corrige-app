<template>
  <display :count="this.number" />
  <buttonCount id="buttonCount" @increment="this.number += 1" />
</template>

<script>
import display from "./components/display.vue";
import buttonCount from "./components/buttonCount.vue";

export default {
  name: "App",
  components: {
    display,
    buttonCount,
  },
  data() {
    return {
      number: 0,
    };
  },
};
</script>

<style lang="scss">
body {
  background-color: #31572c;
  color: white;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#buttonCount {
  position: relative;
  top: 100px;
}
.buttonCount {
  transition-duration: 0.3s;
  background-color: #4f772d;
  padding: 0 20px 0 20px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
}

.buttonCount:hover {
  transition-duration: 0.3s;
  background-color: #132a13;
  transform: scale(0.95);
}

.buttonCount p {
  font-family: "Alfa Slab One", cursive;
  font-size: 30px;
  color: #ecf39e;
}

.conteneur {
  display: flex;
  justify-content: center;
  width: 100%;
}
</style>
