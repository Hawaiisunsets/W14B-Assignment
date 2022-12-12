<template>
    <div>
        <h1>Pick your player</h1>
        <img src="@/assets/user.png" alt="">
        <img src="@/assets/computer.png" alt="">
        <div>
            <button>ROCK</button>
            <button>PAPER</button>
            <button>SCISSOR</button>
        </div>

        

    </div>
</template>

<script>
    export default {
        name : "GameView",
    }
</script>

<style scoped>
img{
    width: 150px;
    height: 150px;
}
</style>