<template>
  <div id="app">
    <div class="buttons-container">
      <button-a color-blue>ボタンA（青）</button-a>
      <button-a color-white>ボタンA（白）</button-a>
      <button-a color-gray>ボタンA（灰）</button-a>
    </div>
    <div class="buttons-container">
      <button-b class="button-blue">ボタンB（青）</button-b>
      <button-b class="button-white">ボタンB（白）</button-b>
      <button-b class="button-gray">ボタンB（灰）</button-b>
    </div>
  </div>
</template>

<script>
import ButtonA from "@/components/ButtonA";
import ButtonB from "@/components/ButtonB";

export default {
  name: "App",
  components: {
    ButtonA,
    ButtonB,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.buttons-container {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: flex-start;
  align-items: flex-start;

  margin: 16px;
}

button {
  margin: 2px;
}
</style>
