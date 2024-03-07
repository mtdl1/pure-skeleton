<template>
  <div class="user-card">
    <div class="card-avatar">
      <img src="../assets/profile.png" alt="" />
    </div>
    <div class="card-info">
      <p class="name">Mateus Dubovicky</p>
      <p class="summary">Olá 👋, meu nome é Mateus Dubovicky e sou Desenvolvedor Front End! Tenho experiência com Vue.js e WordPress, também estudo e me interesso por React e Nuxt!</p>
    </div>
  </div>
</template>

<script setup>
await new Promise((res) => setTimeout(res, 2000));
</script>

<style>
.user-card {
  backdrop-filter: blur(30px);
  background-color: #ffffff6b;
  border: 1px solid rgba(255, 255, 255, .15);
  box-shadow: 0 20px 40px rgba(0,0,0,.05);
  display: flex;
  gap: 30px;
  padding: 20px 40px;
  border-radius: 10px;
}

.card-avatar {
  display: flex;
  align-items: center;
  justify-content: center;
}

.card-avatar img {
  width: 100px;
  height: auto;
  border-radius: 50%;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1),
    0 2px 4px -2px rgb(0 0 0 / 0.1);
}

.card-info {
  display: flex;
  flex: 1;
  flex-direction: column;
  gap: 16px;
}

.name {
  font-size: 32px;
}

.summary {
  font-family: "Lexend", sans-serif;
}

/* responsivo */
@media (max-width: 620px) {
  .user-card {
    width: 90%;
    margin: 0 auto;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
  }
  .card-info p:first-child{
    text-align: center;
  }
  .card-avatar {
    margin: 0 auto;
  }
}
</style>