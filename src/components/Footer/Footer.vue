<script setup>
import FooterNavLi from './FooterNavLi.vue';

</script>

<template>
    <footer>
        <div class="footer-content">
            <nav>
                <ul>
                    <li>
                        <button class="footer-mobile-btn">
                            Platform
                            <svg width="10" viewBox="0 0 10 6" fill="none">
                                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1l4 4 4-4"></path>
                            </svg>
                        </button>
                        <h3 class="footer-desktop-section-link">
                           Platform 
                        </h3>
                        <ul>
                            <li><a href="">Pricing</a></li>
                            <li><a href="">Sign up free</a></li>
                            <li><a href="">Community</a></li>
                            <li><a href="">Website builder</a></li>
                            <li><a href="">Digital products</a></li>
                            <li><a href="">Email marketing</a></li>
                        </ul>
                    </li>
                    <FooterNavLi liName="haha">
                        <li><a href="">1</a></li>
                        <li><a href="">2</a></li>
                        <li><a href="">3</a></li>
                    </FooterNavLi>
                </ul>
            </nav>
        </div>
    </footer>
</template>

