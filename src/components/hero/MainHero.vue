<template>
    <div class="
        relative 
        bg-[#3E3CF0] 
        pt-[80px] 
        rounded-b-[56px] 
        overflow-hidden 
        before:content-['']
        before:absolute 
        before:inset-0 
        before:bg-[linear-gradient(0deg,rgba(26,30,137,1)_0%,rgba(26,30,137,0)_100%)]">
        <Swiper 
            :modules="[Navigation, Autoplay]" 
            :slides-per-view="1" 
            :loop="true"
            :autoplay="{ 
                delay: 3000, 
                disableOnInteraction: false 
            }"
            @swiper="onSwiper">
            <SwiperSlide>
                <div class="relative container mx-auto px-4 z-10">
                    <div class="flex flex-col-reverse md:flex-row pb-40 lg:pb-0">
                        <div class="md:w-1/2">
                            <h2 class="mt-8 sm:mt-15 text-white text-[32px] lg:text-[40px] leading-[40px] lg:leading-[48px] font-light text-center lg:text-left">Hazte cliente empresa del Banco de Chile y <span class="font-bold">obtén tu producto a costo $0*</span></h2>
                            <ul class="flex flex-col items-center lg:flex-row mt-8">
                                <li class="pr-0 pb-5 lg:pr-6 lg:pb-0">
                                    <a class="block py-[16px] px-[24px] bg-[#32FADD] text-[#0A1861] uppercase font-bold rounded-full border border-solid border-[#32FADD] w-[240px] lg:w-auto text-center" href="/">Quiero contratar</a>
                                </li>
                                <li>
                                    <a class="block py-[16px] px-[24px] bg-transparent text-white uppercase font-bold rounded-full border border-solid border-white w-[240px] lg:w-auto text-center" href="/">Nuestras tarifas</a>
                                </li>
                            </ul>
                        </div>
                        <div class="relative md:w-1/2">
                            <img class="absolute w-[196px] sm:w-[300px] md:w-[516px] top-0 right-0 md:right-[-150px] xl:right-[-70px]" :src="slidePhone" alt="Celular">
                            <img class="block m-auto md:m-0 w-[180px] sm:w-[300px] md:w-[474px]" :src="slidePerson" alt="Persona">
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="relative container mx-auto px-4 z-10">
                    <div class="flex flex-col-reverse md:flex-row pb-40 lg:pb-0">
                        <div class="md:w-1/2">
                            <h2 class="mt-8 sm:mt-15 text-white text-[32px] lg:text-[40px] leading-[40px] lg:leading-[48px] font-light text-center lg:text-left">Hazte cliente empresa del Banco de Chile y <span class="font-bold">obtén tu producto a costo $0*</span></h2>
                            <ul class="flex flex-col items-center lg:flex-row mt-8">
                                <li class="pr-0 pb-5 lg:pr-6 lg:pb-0">
                                    <a class="block py-[16px] px-[24px] bg-[#32FADD] text-[#0A1861] uppercase font-bold rounded-full border border-solid border-[#32FADD] w-[240px] lg:w-auto text-center" href="/">Quiero contratar</a>
                                </li>
                                <li>
                                    <a class="block py-[16px] px-[24px] bg-transparent text-white uppercase font-bold rounded-full border border-solid border-white w-[240px] lg:w-auto text-center" href="/">Nuestras tarifas</a>
                                </li>
                            </ul>
                        </div>
                        <div class="relative md:w-1/2">
                            <img class="absolute w-[196px] sm:w-[300px] md:w-[516px] top-0 right-0 md:right-[-150px] xl:right-[-70px]" :src="slidePhone" alt="Celular">
                            <img class="block m-auto md:m-0 w-[180px] sm:w-[300px] md:w-[474px]" :src="slidePerson" alt="Persona">
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="relative container mx-auto px-4 z-10">
                    <div class="flex flex-col-reverse md:flex-row pb-40 lg:pb-0">
                        <div class="md:w-1/2">
                            <h2 class="mt-8 sm:mt-15 text-white text-[32px] lg:text-[40px] leading-[40px] lg:leading-[48px] font-light text-center lg:text-left">Hazte cliente empresa del Banco de Chile y <span class="font-bold">obtén tu producto a costo $0*</span></h2>
                            <ul class="flex flex-col items-center lg:flex-row mt-8">
                                <li class="pr-0 pb-5 lg:pr-6 lg:pb-0">
                                    <a class="block py-[16px] px-[24px] bg-[#32FADD] text-[#0A1861] uppercase font-bold rounded-full border border-solid border-[#32FADD] w-[240px] lg:w-auto text-center" href="/">Quiero contratar</a>
                                </li>
                                <li>
                                    <a class="block py-[16px] px-[24px] bg-transparent text-white uppercase font-bold rounded-full border border-solid border-white w-[240px] lg:w-auto text-center" href="/">Nuestras tarifas</a>
                                </li>
                            </ul>
                        </div>
                        <div class="relative md:w-1/2">
                            <img class="absolute w-[196px] sm:w-[300px] md:w-[516px] top-0 right-0 md:right-[-150px] xl:right-[-70px]" :src="slidePhone" alt="Celular">
                            <img class="block m-auto md:m-0 w-[180px] sm:w-[300px] md:w-[474px]" :src="slidePerson" alt="Persona">
                        </div>
                    </div>
                </div>
            </SwiperSlide>
        </Swiper>
        <div class="absolute container mx-auto px-4 bottom-[60px] lg:bottom-[100px] left-0 right-0 z-10">
            <ul class="flex justify-center lg:justify-start">
                <li class="pr-3">
                    <button @click="slidePrev" class="flex justify-center items-center w-[56px] h-[56px] rounded-full bg-[rgba(10,24,97,.8)] cursor-pointer">
                        <img class="block" :src="iconArrowPrev" alt="Atras">
                    </button>
                </li>
                <li class="pr-3">
                    <button @click="slideNext" class="flex justify-center items-center w-[56px] h-[56px] rounded-full bg-[rgba(10,24,97,.8)] cursor-pointer">
                        <img class="block" :src="iconArrownext" alt="Siguiente">
                    </button>
                </li>
                <li>
                    <button @click="toggleAutoplay" class="flex justify-center items-center w-[56px] h-[56px] cursor-pointer" :aria-label="isPlaying ? 'Pausar' : 'Reproducir'">
                        <img v-if="isPlaying" class="block" :src="iconPause" alt="Pausar">
                        <span v-else class="block text-white text-[18px]">▶</span>
                    </button>
                </li>
            </ul>
        </div>
        <img class="absolute w-[300px] sm:w-[400px] md:w-[500px] xl:w-auto top-[-100px] right-[-70px]" :src="shapeBg" alt="Shape">
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    import { Swiper, SwiperSlide } from 'swiper/vue'
    import { Navigation, Autoplay } from 'swiper/modules'
    import 'swiper/css'
    import 'swiper/css/navigation'
    import 'swiper/css/pagination'

    const swiperInstance = ref(null)
    const isPlaying = ref(false)

    const onSwiper = (swiper) => {
        swiperInstance.value = swiper
    }

    const slidePrev = () => {
        if (swiperInstance.value) {
            swiperInstance.value.slidePrev()
        }
    }

    const slideNext = () => {
        if (swiperInstance.value) {
            swiperInstance.value.slideNext()
        }
    }

    const toggleAutoplay = () => {
        if (swiperInstance.value) {
            if (isPlaying.value) {
                swiperInstance.value.autoplay.stop()
                isPlaying.value = false
            } else {
                swiperInstance.value.autoplay.start()
                isPlaying.value = true
            }
        }
    }

    import shapeBg from '@/assets/images/resources/slide-bg-shape.svg'
    import slidePerson from '@/assets/images/resources/slide-person.png'
    import slidePhone from '@/assets/images/resources/slide-phone.png'
    import iconArrowPrev from '@/assets/images/icons/icon-arrow-prev.svg'
    import iconArrownext from '@/assets/images/icons/icon-arrow-next.svg'
    import iconPause from '@/assets/images/icons/icon-pause.svg'
</script>