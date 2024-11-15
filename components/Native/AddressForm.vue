<script setup lang="ts"></script>

<template>
    <form method="post" action="/api/address">
        <label for="name">Full name</label>
        <input type="text" name="name" />

        <label for="email">Email</label>
        <input type="email" name="email" />

        <label for="phone">Phone</label>
        <input type="tel" name="phone" />

        <label for="streetName">Street name</label>
        <input type="text" name="streetName" />

        <label for="city">City</label>
        <input type="text" name="city" />

        <NativeCountryInput />

        <label for="isDefault">Mark as default address</label>
        <input type="checkbox" name="isDefault" />

        <input type="submit" value="Submit">
    </form>
</template>

<style scoped lang="postcss">
input {
    @apply border p-2;
}
</style>