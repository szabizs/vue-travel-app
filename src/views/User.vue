<template>
    <div>
        <h1>User Page</h1>
        <button v-on:click="logout" class="btn">Logout</button>
        <p>
            <router-link :to="{name: 'invoices'}">Invoices</router-link>
        </p>
    </div>
</template>
<script>
import store from '@/store'

export default {
    methods: {
        logout(){
            store.user = null;
            this.$router.push("/")
        }
    }
}
</script>