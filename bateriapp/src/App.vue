<template>
  <div>VUE BATERİ</div>
  <div class="keys">
    <Key v-for="(key, i) in keys" :sound="key" :key="i" />
  </div>
</template>

<script>
import Key from "./components/Key.vue";
export default {
  name: "App",
  data() {
    return {
      keys: [
        {
          name: "boom",
          audio: require("./assets/sounds/1.mp3"),
          letter: "W",
        },
        {
          name: "clap",
          audio: require("./assets/sounds/2.mp3"),
          letter: "S",
        },
        {
          name: "hithat",
          audio: require("./assets/sounds/3.mp3"),
          letter: "D",
        },
        {
          name: "kick",
          audio: require("./assets/sounds/4.mp3"),
          letter: "F",
        },
        {
          name: "openhat",
          audio: require("./assets/sounds/5.mp3"),
          letter: "G",
        },
        {
          name: "ride",
          audio: require("./assets/sounds/6.mp3"),
          letter: "H",
        },
        {
          name: "wow",
          audio: require("./assets/sounds/7 .mp3"),
          letter: "A",
        },
        {
          name: "low",
          audio: require("./assets/sounds/8.mp3"),
          letter: "Q",
        },
        {
          name: "justin",
          audio: require("./assets/sounds/9.mp3"),
          letter: "J",
        },
        {
          name: "bilge",
          audio: require("./assets/sounds/10.mp3"),
          letter: "B",
        },
        {
          name: "yey",
          audio: require("./assets/sounds/11.mp3"),
          letter: "Y",
        },
        {
          name: "oww",
          audio: require("./assets/sounds/12.mp3"),
          letter: "O",
        },
        {
          name: "puf",
          audio: require("./assets/sounds/13.mp3"),
          letter: "P",
        },
        {
          name: "uff",
          audio: require("./assets/sounds/14.mp3"),
          letter: "U",
        },
        {
          name: "fight",
          audio: require("./assets/sounds/15.mp3"),
          letter: "I",
        },
        {
          name: "put",
          audio: require("./assets/sounds/16.mp3"),
          letter: "T",
        },
        {
          name: "bom",
          audio: require("./assets/sounds/17.mp3"),
          letter: "M",
        },
        {
          name: "blop",
          audio: require("./assets/sounds/18.mp3"),
          letter: "L",
        },
        {
          name: "pat",
          audio: require("./assets/sounds/19.mp3"),
          letter: "K",
        },
      ],
    };
  },
  components: {
    Key,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #3a0ca3;
  margin-top: 60px;
  font-size: 80px;
}
.keys {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
