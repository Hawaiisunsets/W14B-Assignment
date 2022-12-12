<template>
    <div>
        <GameScoreboard/>
        <GameUser/>
        <GameComputer/>
    </div>
</template>

<script>
import GameScoreboard from "@/components/GameScoreboard.vue";
import GameUser from "@/components/GameUser.vue";
import GameComputer from "@/components/GameComputer.vue";

    export default {
        name : "GameScreen",
        components : {
            GameScoreboard,
            GameUser,
            GameComputer
        },
        // data (){
        //     return{
        //         counter
        //     }
        // }
    }
</script>

<style scoped>

</style>