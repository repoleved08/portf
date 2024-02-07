<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
import Jumbotron from './views/Jumbotron.vue';
import AboutMe from '@/views/AboutMe.vue';
import MyOffer from '@/views/MyOffer.vue';
import MyServices from '@/views/MyServices.vue';
import TimeLine from '@/components/TimeLine.vue';
import Accordion from './views/Accordion.vue';

//others
import { useDark, useToggle } from '@vueuse/core';

const isDark = useDark();
const toggleDark = useToggle(isDark);

</script>

<template>
  
  <Navbar :isDark="isDark" :toggleDark="toggleDark"/>
  <Jumbotron/>
  <AboutMe/>
  <MyOffer/>
  <MyServices/>
  <TimeLine/>
  <Accordion/>
  <RouterView />
  <Footer/>
</template>


