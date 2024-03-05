<template>
  <div class="placeholder">
    &nbsp;
  </div>
</template>

<script setup>
defineProps({
  width: {
    type: String,
    default: '100%',
  },
  height: {
    type: String,
    default: '100%',
  },
  borderRadius: {
    type: String,
    default: '0',
  },
});
</script>

<style scoped>
@keyframes pulse {
  0% {
    background-position: 0% 0%;
  }
  100% {
    background-position: -135% 0%;
  }
}
.placeholder {
  width: v-bind(width);
  height: v-bind(height);
  border-radius: v-bind(borderRadius);
  background-image: linear-gradient(
    90deg,
    #f1f1f1 25%,
    #e1e1e1 37%,
    #f1f1f1 63%
  );
  background-size: 400% 400%;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1),
    0 2px 4px -2px rgb(0 0 0 / 0.1);
  animation: pulse 1.5s linear infinite;
}
</style>