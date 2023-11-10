<template>
        <HeroHeader />
        <Stats />
        <AboutUs />
        <About />
        <Attachment />
        <Team />
        <Example/>
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
import Example from '@/components/section/Example.vue'
export default{
    components:{HeroHeader,About,Stats,Team,Contact,Footer,Example,AboutUs,Attachment}
}
</script>