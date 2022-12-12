<template>
    <div>
        <!-- <router-link to="/">Login</router-link> -->
        <!-- <div class="divLogin">
            <input v-model="userName" type="text" placeholder="username">
            <input v-model="userPassword" type="text" placeholder="password">
            <button @click="getLogin">Login</button>
        </div> -->
    </div>
</template>

<script>
// import axios from 'axios';
// import cookies from 'vue-cookies';

    export default {
        name : "LoginApp",
        // data(){
        //     return{
        //         userName : "",
        //         userPassword : ""
        //     }
        // },
        // methods : {
        //     getLogin(){
        //         axios.request({
        //             url : "https://reqres.in/api/login",
        //             method : "POST",
        //             data : {
        //                 email : this.userName,
        //                 password : this.userPassword
        //             }
        //         }).then((response)=>{
        //             console.log(response);
        //             let getToken = response.data.token
        //             cookies.set(`loginToken`, getToken);
        //             document.location.href = "/game";
        //         }).catch((error)=>{
        //             console.log(error);
        //             // insert message if unsuccessfull login
        //             document.querySelector(`button`).insertAdjacentHTML(`beforebegin`, `<p>Please Try Again!</p>`);
        //         })
        //     },
        // }
        
    }
</script>

<style scoped>
.divLogin{
    margin-top: 100px;
}
</style>