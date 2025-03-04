<template>
  <main>
    <ChessBoard/>
  </main>
</template>

<script setup>
  import ChessBoard from './components/ChessBoard.vue';
</script>


<style>
  main {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  main > * {
    width: 50%;
  }
</style>
