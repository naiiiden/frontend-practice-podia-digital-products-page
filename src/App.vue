<script setup>
import Header from './components/Header/Header.vue';
import { openDropdown } from './components/Header/openDropdown';
import Hero from './components/Hero/Hero.vue';
</script>

<template>
  <Header/>
  <div @click="openDropdown = !openDropdown">
    <main>
      <Hero 
        headingPreText="Digital Products"
        heading1="Sell online courses, coaching sessions, webinars, workshops, ebooks, and anything you can think of on Podia"
        paragraph="Get everything you need in one place that you own. Podia takes care of hosting products, taking payments, and getting products to your customers. And you always control your own work."
        link="Get your free account"  
        img="src/assets/digital_products-hero.png"
      />
      
      <Hero 
        headingPreText="Online Courses"
        heading2="Beautiful online courses you can build in moments"
        paragraph="Make a beautiful online course for your customers. Podia hosts your course. That means all the lessons, files, and videos you want handled for you."
        linkSecondary="Learn more about courses"  
        img="src/assets/digital_products-courses.png"
      />

      <Hero 
        headingPreText="Digital Downloads"
        heading2="Ebooks, templates, and any file type you can think of"
        paragraph="Have an ebook to sell? Templates you love? Podia makes it easy to spin up a sales page and sell ebooks, templates, audio files, video files, spreadsheets, and any other file type."
        linkSecondary="Learn more about downloads"  
        img="src/assets/digital_products-downloads.png"
      />

      <Hero 
        headingPreText="Coaching"
        heading2="One-on-one coaching and consultations, with billing managed for you"
        paragraph="Sometimes your students want one-on-one attention. Podia makes it easy for you to charge for coaching sessions and consultations."
        linkSecondary="Learn more about coaching"  
        img="src/assets/digital_products-coaching.png"
      />

      <Hero 
        headingPreText="Webinars"
        heading2="Webinars and workshops with registration and payment in one place"
        paragraph="How can you charge for your webinars and workshops? Do it from your Podia site. Set up a paid webinar product and your customers can register straight from your website."
        linkSecondary="Learn more about webinars"  
        img="src/assets/digital_products-webinars.png"
      />
    </main>
  </div>
</template>