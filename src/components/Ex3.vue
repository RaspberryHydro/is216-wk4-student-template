<script setup>
    import { ref } from 'vue'

    // Add code here
    const loginoption = ref('username')
    
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="loginoption">
        <option selected name="login" value="username">Username login</option>
        <option name="login" value="email">Email login</option>
    </select>
    
    <div v-if="loginoption === 'username'">
        <label>Username</label>
        <input placeholder="Enter your username">
    </div>
    <div v-if="loginoption === 'email'">
        <label>email</label>
        <input  placeholder="Enter your email address">
    </div>
</template>

