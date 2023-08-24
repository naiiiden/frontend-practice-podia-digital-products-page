<script setup>
import FooterNavLi from './FooterNavLi.vue';

const footerNavList = ref([
    {
        liName: 'Platform',
        links: [
            {
                href: '',
                text: 'Pricing',
            },
            {
                href: '',
                text: 'Sign up free',
            },
            {
                href: '',
                text: 'Community',
            },
            {
                href: '',
                text: 'Website builder',
            },
            {
                href: '',
                text: 'Digital products',
            },
            {
                href: '',
                text: 'Email marketing',
            },
        ]
    }, 
    {
        liName: 'Support',
        links: [
            {
                href: '',
                text: 'Contact us',
            },
            {
                href: '',
                text: 'Help center',
            },
            {
                href: '',
                text: 'Hire a Podia pro',
            },
            {
                href: '',
                text: 'Creator community',
            },
            {
                href: '',
                text: 'Podia 101',
            },
        ]
    },
    {
        liName: 'Features',
        links: [
            {
                href: '',
                text: 'Online courses',
            },
            {
                href: '',
                text: 'Downloads',
            },
            {
                href: '',
                text: 'Webinars',
            },
            {
                href: '',
                text: 'Coaching',
            },
            {
                href: '',
                text: 'All features',
            },
        ]
    },
    {
        liName: 'Compare',
        links: [
            {
                href: '',
                text: 'Kajabi',
            },
            {
                href: '',
                text: 'Teachable',
            },
            {
                href: '',
                text: 'Thinkific',
            },
            {
                href: '',
                text: 'Patreon',
            },
            {
                href: '',
                text: 'Gumroad',
            },
            {
                href: '',
                text: 'Podia alternatives',
            },
        ]
    }, 
    {
        liName: 'Resources',
        links: [
            {
                href: '',
                text: 'Examples',
            },
            {
                href: '',
                text: 'Demo',
            },
            {
                href: '',
                text: 'Creator stories',
            },
            {
                href: '',
                text: 'Blog',
            },
            {
                href: '',
                text: 'Free tools',
            },
            {
                href: '',
                text: 'All resources',
            },
        ]
    },
    {
        liName: 'Podia',
        links: [
            {
                href: '',
                text: 'Jobs',
            },
            {
                href: '',
                text: 'About',
            },
            {
                href: '',
                text: 'Branding',
            },
            {
                href: '',
                text: 'Reviews',
            },
            {
                href: '',
                text: 'Refer-a-creator',
            },
            {
                href: '',
                text: 'Affiliates',
            },
        ]
    },
    {
        liName: 'Social',
        links: [
            {
                href: '',
                text: 'Twitter',
            },
            {
                href: '',
                text: 'Facebook',
            },
            {
                href: '',
                text: 'Instagram',
            },
            {
                href: '',
                text: 'Youtube',
            },
        ]
    }
])
</script>

<template>
    <footer>
        <div class="footer-content">
            <nav>
                <ul>
                    <FooterNavLi liName="Social">
                        <li><a href="">Twitter</a></li>
                        <li><a href="">Facebook</a></li>
                        <li><a href="">Instagram</a></li>
                        <li><a href="">Youtube</a></li>
                    </FooterNavLi>
                </ul>
            </nav>
        </div>
    </footer>
</template>

