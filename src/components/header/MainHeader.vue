<script setup>
    import NavMenu from './NavMenu.vue';
    import ButtonHire from './ButtonHire.vue';

    import logo from '@/assets/images/logo.svg'
</script>

<template>
    <header class="py-3 bg-[#1A1E89]">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center">
                <a href="/" class="block">
                    <img :src="logo" alt="Pago de Banco de Chile">
                </a>
                <NavMenu class="order-last md:order-0" />
                <ButtonHire />
            </div>
        </div>
    </header>
</template>