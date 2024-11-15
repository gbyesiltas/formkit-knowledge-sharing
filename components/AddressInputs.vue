<template>
    <FormKit type="text" name="street" label="Street" />
    <FormKit type="text" name="city" label="City" />
    <FormKit type="select" name="country" :options="[{ label: 'Netherlands', value: 'nl' }, { label: 'United Kingdom', value: 'uk' }]" />
</template>