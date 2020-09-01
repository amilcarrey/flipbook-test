<template>
  <div id="app">
    <Flipbook class="flipbook" :pages="pages" v-slot="flipbook" ref="flipbook"></Flipbook>
  </div>
</template>

<script>
import Flipbook from "flipbook-vue";
export default {
  components: {
    Flipbook
  },
  data: () => {
    return {
      pages: [
        "https://images.pexels.com/photos/4380970/pexels-photo-4380970.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260",
        "https://images.pexels.com/photos/2709385/pexels-photo-2709385.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/2709385/pexels-photo-2709385.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/3081752/pexels-photo-3081752.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/3083250/pexels-photo-3083250.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      ],
      pagesHiRes: [
        "https://images.pexels.com/photos/4380970/pexels-photo-4380970.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260",
        "https://images.pexels.com/photos/2709385/pexels-photo-2709385.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/2709385/pexels-photo-2709385.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/3081752/pexels-photo-3081752.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/3083250/pexels-photo-3083250.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      ]
    };
  }
};
</script>

<style>
html,
body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #333;
  color: #ccc;
  overflow: hidden;
}
.flipbook {
  width: 60vw;
  height: calc(100vh - 50px - 40px);
}
.flipbook .bounding-box {
  box-shadow: 0 0 20px #000;
}
</style>
