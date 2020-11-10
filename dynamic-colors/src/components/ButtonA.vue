<template>
  <button :style="buttonStyle">
    <slot></slot>
  </button>
</template>

<script>
export default {
  computed: {
    buttonStyle: {
      get() {
        let buttonBgColor = "blue";
        let buttonColor = "white";
        if (this.colorWhite) {
          buttonBgColor = "white";
          buttonColor = "black";
        }
        if (this.colorGray) {
          buttonBgColor = "gray";
          buttonColor = "white";
        }

        return `background-color: ${buttonBgColor}; color: ${buttonColor};`;
      },
    },
  },
  name: "ButtonA",
  props: {
    colorBlue: {
      type: Boolean,
      required: false,
      default: false,
    },
    colorWhite: {
      type: Boolean,
      required: false,
      default: false,
    },
    colorGray: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
};
</script>

<style>
</style>