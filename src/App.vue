<script setup>
import Header from './components/Header/Header.vue';
import { openDropdown } from './components/Header/openDropdown';
import Hero from './components/Hero/Hero.vue';
import SectionHeading from './components/SectionHeading/SectionHeading.vue';
import FeatureCard from './components/FeatureCard/FeatureCard.vue';
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
      <section>
        <SectionHeading 
          heading="All you have to do is make the product. Podia takes care of the details for you."
          paragraph="Podia lets you make your sales page, take payments, and give your customers access all in one place. Host and sell your products without needing to figure out a handful of new tools."  
        />
        <div class="feature-cards-container">
          <FeatureCard 
            img="src/assets/cart.svg"
            h3="Checkout and sales are handled for you"
            paragraph="You don’t have to figure out a bunch of tools or website embeds. Just connect a payment provider and your Podia site takes care of payments for you."  
          />
          <FeatureCard 
            img="src/assets/login.svg"
            h3="Your customers log in, and your products are there for them"
            paragraph="Your Podia site handles access to products for you. Everything is in one place. When your customers buy a product, they get a log in. After that, they can see all the products they’ve bought from you."  
          />
          <FeatureCard 
            img="src/assets/cloud.svg"
            h3="Upload your product. Make your sales page. Done."
            paragraph="You could sell a digital product by this afternoon. Podia handles hosting, sales pages, checkout, and delivery. All you need is something to sell."  
          />
        </div>
      </section>
      <section>
        <SectionHeading
          heading="What kinds of products can you sell with Podia?"
          paragraph="Podia gives you the flexibility to sell whatever you want. That means you have more ways to grow your creator business."
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
      </section>
    </main>
  </div>
</template>