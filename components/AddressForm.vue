<script setup lang="ts">
const onSubmit = (formData: { name: string, email: string, country: string }) => {
    console.log(formData);
}
</script>

<template>
    <!-- 
        - type
        - name and id
        - placeholder
        - help
    -->
    <FormKit type="form" @submit="onSubmit">
        <FormKit type="group" name="person">
            <FormKit type="text" name="name" label="Name" placeholder="Enter your full name" />
            <FormKit type="email" name="email" label="Email" help="We won't send you emails" />
        </FormKit>
        
        <FormKit type="group" name="address">
            <AddressInputs />
        </FormKit>
    </FormKit>
</template>

<style lang="postcss">
input {
    @apply border p-2;
}
</style>