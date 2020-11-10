<template>
  <button>
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "ButtonB",
};
</script>

<style>
button.button-blue {
  background-color: blue;
  color: white;
}
button.button-white {
  background-color: white;
  color: black;
}
button.button-gray {
  background-color: gray;
  color: white;
}
</style>