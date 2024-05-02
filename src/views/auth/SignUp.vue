<script setup>
import UsernameField from "../../components/UsernameField.vue";
import EmailField from "../../components/EmailField.vue";
import PasswordField from "../../components/PasswordField.vue";
</script>

<template>
  <div class="p-8">
    <h1 class="mb-6">Sign Up</h1>

    <UsernameField />
    <EmailField />
    <PasswordField />
  </div>
</template>
