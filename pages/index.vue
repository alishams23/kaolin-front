<template>
        <HeroHeader />
        <Stats />
        <AboutUs />
        <About />
        <Application/>
        <Attachment />
        <Team class="mb-10" />
        <Contact/>
        <Footer/>
</template>

<script>
import HeroHeader from '@/components/section/HeroHeader.vue'
import Stats from '@/components/section/Stats.vue'
import AboutUs from '@/components/section/AboutUs.vue'
import About from '@/components/section/About.vue'
import Team from '@/components/section/Team.vue'
import Contact from '@/components/section/Contact.vue'
import Attachment from '@/components/section/Attachment.vue'
import Footer from '@/components/section/Footer.vue'
import Application from '@/components/section/Application.vue'
export default{
    components:{HeroHeader,About,Stats,Team,Contact,Footer,Application,AboutUs,Attachment}
}
</script>