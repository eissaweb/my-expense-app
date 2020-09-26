<template>
    <form class="form-signin" @submit.prevent="register">
    <h1 class="h3 mb-3 font-weight-normal">Please Register</h1>
     <label for="name" class="sr-only">Name</label>
    <input type="text" id="name" class="form-control" placeholder="Name" required="" v-model="input.name">
    <label for="inputEmail" class="sr-only">Email address</label>
    <input type="email" id="inputEmail" class="form-control" placeholder="Email address" required="" autofocus="">
    <label for="inputPassword" class="sr-only">Enter Password</label>
    <input type="password" id="inputPassword" class="form-control" placeholder="Password" required="">
     <label for="inputPassword" class="sr-only">Confirm Password</label>
    <input type="password" id="inputPassword" class="form-control" placeholder="Confirm Password" required="">
    <br/>
    <button class="btn btn-lg btn-primary btn-block" type="submit">Register</button>
    <p class="text-muted">
        Have an account? 
        <router-link to="/login"> Login</router-link>
    </p>
</form>
</template>

<script>
export default {
    data() {
        return {
            input: {
                name: '',
                password: '',
                password_confirmation: '',
                email: ''
            }
        }
    },
    methods: {
        register() {
            console.log('done.');
        }
    }
}
</script>