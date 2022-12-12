<template>
    <div>
        <h1>WELCOME PLAYER</h1>
        <div class="divLogin">
            <input v-model="userName" type="text" placeholder="username">
            <input v-model="userPassword" type="text" placeholder="password">
            <button @click="getLogin">Login</button>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
import cookies from 'vue-cookies';
import router from "@/router";

    export default {
        name : "LoginView",
        data(){
            return{
                userName : "",
                userPassword : ""
            }
        },
        methods : {
            getLogin(){
                axios.request({
                    url : "https://reqres.in/api/login",
                    method : "POST",
                    data : {
                        email : this.userName,
                        password : this.userPassword
                    }
                }).then((response)=>{
                    console.log(response);
                    let getToken = response.data.token
                    cookies.set(`loginToken`, getToken);
                    router.push(`/game`);
                }).catch((error)=>{
                    console.log(error);
                    // insert message if unsuccessfull login
                    document.querySelector(`button`).insertAdjacentHTML(`beforebegin`, `<p>Please Try Again!</p>`);
                })
            },
        }
        
    }
</script>

<style scoped>
.divLogin{
    margin-top: 100px;
}
</style>