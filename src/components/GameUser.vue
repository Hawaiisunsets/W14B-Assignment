<template>
    <div>
        <!-- <img src="@/assets/user.png" alt=""> -->
    </div>
</template>

<script>
    export default {
        name: "GameUser",
        data(){
            return{
                pickUser: "",
                PickComputer: "",
                randomNumber: "",
                pictureUser: "user.png",
                choices: [
                    {
                        id: 0,
                        choiceName: "Rock",
                        beats: "Scissors",
                        computerChoice: "",
                        url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTd6eB8VomN8uaD7gFZvHhqVIoTQJC658HsvA&usqp=CAU"
                    },
                    {
                        id: 1,
                        choiceName: "Paper",
                        beats: "Rock",
                        computerChoice: "",
                        url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe_KMA1Z7FzH29EoUC8E2t5Tu_M736jp7uFw&usqp=CAU"
                    },
                    {
                        id: 2,
                        choiceName: "Scissor",
                        beats: "Paper",
                        computerChoice: "",
                        url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcROfc_UC01fXzwWYu3CAZocv6l_XXWz3pFv7Q&usqp=CAU'
                    },
                ]
            }
        },
        methods: {
            
        }
    }
</script>

<style scoped>
img{
    width: 150px;
    height: 150px;
}
</style>