<template>
    <section id="board">
        <div class="square" v-for="i in 8" :key="i">
            <div class="piece" v-for="j in 8" :key="j" :class="i % 2 === j % 2 ? 'white' : 'black'">
    
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped>
    #board {
        display: block;
        border: 1px solid black;
        aspect-ratio: 1;
        margin: 40px;
    }

    .square {
        display: grid;
        grid-template-columns: repeat(8, 1fr);
        width: 100%;
        height: calc(100% / 8);
    }

    .black {
        background-color: #8B4513;
    }

    .white {
        background-color: #FFDAB9;
    }
</style>