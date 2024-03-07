<template>
  <div>
    <div class="user-card">
      <div class="card-avatar">
        <AnimatedPlaceholder width="100px" height="100px" borderRadius="50%" />
      </div>
      <div class="card-info">
        <AnimatedPlaceholder width="30%" height="32px" borderRadius="4px" class="titulo"/>
        <div class="summary-placeholder">
          <AnimatedPlaceholder width="100%" height="18px" borderRadius="4px" />
          <AnimatedPlaceholder width="100%" height="18px" borderRadius="4px" />
          <AnimatedPlaceholder width="100%" height="18px" borderRadius="4px" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import AnimatedPlaceholder from './AnimatedPlaceholder.vue';
</script>

<style scoped>
.summary-placeholder{
  display: flex;
  flex-direction: column;
  gap: 8px;
  width: 100%;
}
.titulo{
  margin: 0 auto;
}
</style>