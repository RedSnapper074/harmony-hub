<template>
    <div class="register">
        <img class="logo" src="../assets/bane.jpg" />
        <h1>Welcome to HarmonyHub</h1>
        <input type="email" v-model="email" placeholder="Enter Email" >
        <input type="password" v-model="password" placeholder="Enter Password" >
        <button @click="register">Register</button>
    </div>
</template>

<script>
import AuthenticationService from '@/services/AuthenticationService'
export default {
    name: 'Register',
    data()
    {
        return {
            email:'',
            password:''
        }
    },
    
    methods: {
        async register(){
            const response = await AuthenticationService.register({
                email: this.email,
                password: this.password
            })
            console.log(response.data)
        }
    }
    
}
</script>
