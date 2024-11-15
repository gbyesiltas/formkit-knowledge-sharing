<template>
    <!-- 
        - type
        - name and id
        - placeholder
        - help
    -->
    <FormKit type="form">
        <FormKit type="text" name="name" label="Name" placeholder="Enter your full name" />
        <FormKit type="email" name="email" label="Email" help="We won't send you emails" />
        <FormKit type="select" name="country" :options="[{ label: 'Netherlands', value: 'nl' }, { label: 'United Kingdom', value: 'uk' }]" />
    </FormKit>
</template>

<style lang="postcss">
input {
    @apply border p-2;
}
</style>