<template>
    <section class="images">
        <article class="main-images">
            <img v-if="active[0]" :src="image1" alt="">
            <img v-if="active[1]" :src="image2" alt="">
            <img v-if="active[2]" :src="image3" alt="">
        </article>
        <article class="thumbnails">
            <img :src="thumb1" :class="{active: active[0], thumnail: true}" @click="toggleActive(0)" alt="thumnail">
            <img :src="thumb2" :class="{active: active[1], thumnail: true}" @click="toggleActive(1)" alt="thumnail">
            <img :src="thumb3" :class="{active: active[2], thumnail: true}" @click="toggleActive(2)" alt="thumnail">
        </article>
    </section>
</template>

<script setup>
import '@/assets/styles/ProductImages.scss';
import thumb1 from '@/assets/images/brown2.png';
import thumb2 from '@/assets/images/white2.png';
import thumb3 from '@/assets/images/black3.png';
import image1 from '@/assets/images/brown1.png';
import image2 from '@/assets/images/white1.png';
import image3 from '@/assets/images/black1.png';
import { ref } from 'vue';

const active = ref([true, false, false])
function toggleActive(index) {
    active.value = active.value.map((value,i) => i === index)
}

</script>
