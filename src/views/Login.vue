<template>
    <div class="w-md-75">
    <form class="form-signin" @submit.prevent="login">
        <h1 class="h3 mb-3 font-weight-normal">Please sign in</h1>
    <label for="inputEmail" class="sr-only">Email address</label>
    <input type="email" id="inputEmail" class="form-control" v-model="input.email" placeholder="Email address" required="" autofocus="">
    <label for="inputPassword" class="sr-only">Password</label>
    <input type="password" id="inputPassword" class="form-control" v-model="input.password" placeholder="Password" required="">
    <div class="checkbox mb-3">
        <label>
        <input type="checkbox" value="remember-me"> Remember me
        </label>
    </div>
    <button class="btn btn-lg btn-primary btn-block" type="submit">Log in</button>
    <p class="text-muted">
        Haven't registered yet ? 
        <router-link to="/register"> Register</router-link>
    </p>
    </form>
    </div>
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
        login() {
            console.log('login.');
        }
    }
}
</script>