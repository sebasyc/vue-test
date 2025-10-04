<script setup>
    import iconHamburguer from '@/assets/images/icons/icon-hamburguer.svg'
</script>

<template>
    <nav>
        <div class="hidden md:block">
            <ul class="flex items-center space-x-8">
                <li>
                    <a href="/" class="uppercase text-white text-xs font-semibold">Productos y tarifas</a>
                </li>
                <li>
                    <a href="/" class="uppercase text-white text-xs font-semibold">Como contratar</a>
                </li>
                <li>
                    <a href="/" class="uppercase text-white text-xs font-semibold">Beneficios</a>
                </li>
            </ul>
        </div>
        
        <div class="md:hidden ml-3 md:ml-0">
            <button class="block">
                <img :src="iconHamburguer" alt="Icon Hamburguesa">
            </button>  
        </div>
    </nav>
</template>