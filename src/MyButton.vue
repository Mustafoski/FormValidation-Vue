<template>
  <div>
    <button :style="{ background, color }" :disabled="disabled">Button</button>
  </div>
</template>

<script>
export default {
  name: 'MyButton',
  props: {
    background: String,
    color: String,
    disabled: Boolean,
  },
};
</script>

<style scoped>
button:disabled {
  opacity: 0.5;
}

button {
  background: none;
  color: black;
  border: none;
  border-radius: 5px;
  padding: 10px 40px;
  font-size: 16px;
  cursor: pointer;
}
button:hover {
  filter: brightness(125%);
}
</style>
