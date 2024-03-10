<template>
  <div>
    <main>
      <Suspense>
        <UserCard />
        <template #fallback>
          <UserCardSkeleton />
        </template>
      </Suspense>
    </main>
  </div>
</template>

<script setup>
import UserCard from './components/UserCard.vue';
import UserCardSkeleton from './components/UserCardSkeleton.vue';

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Anta&family=Lexend:wght@100..900&display=swap');

*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: "Anta", sans-serif;
}

body{
  background-color: #F1F2EE;
}

main{
  max-width: 620px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  gap: 16px;
  height: 100dvh;
  justify-content: center;
}
</style>