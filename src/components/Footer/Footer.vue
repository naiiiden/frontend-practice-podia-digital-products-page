<script setup>
import FooterNavLi from './FooterNavLi.vue';
import { ref } from 'vue';

// ChatGPT
const dropdownStates = ref({});

const toggleDropdown = (dropdownName) => {
  Object.keys(dropdownStates.value).forEach((dropdown) => {
    // Close all other dropdowns except the clicked one
    if (dropdown !== dropdownName) {
      dropdownStates.value[dropdown] = false;
    }
  });

  // Toggle the state of the clicked dropdown
  dropdownStates.value[dropdownName] = !dropdownStates.value[dropdownName];
};

const isDropdownOpen = (dropdownName) => dropdownStates.value[dropdownName];

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
                <ul class="footer-content-mobile">
                    <FooterNavLi
                        v-for="linkSection in footerNavList"
                        :key="linkSection.liName"
                        :liName="linkSection.liName"
                        @toggleDropdown="toggleDropdown"
                    >
                        <ul v-if="isDropdownOpen(linkSection.liName)">
                            <li v-for="link in linkSection.links" :key="link.text">
                                <a href="">{{ link.text }}</a>
                            </li>
                        </ul>
                    </FooterNavLi>
                </ul>
                <ul class="footer-content-desktop">
                    <FooterNavLi v-for="linkSection in footerNavList" :liName='linkSection.liName'>
                        <ul>
                            <li v-for="link in linkSection.links">
                                <a href="">{{ link.text }}</a>
                            </li>
                        </ul>
                    </FooterNavLi>
                </ul>
            </nav>
            <div>
                <p>Podia Labs, Inc. © 2023</p>
                <ul>
                    <li><a href="">Terms</a></li>
                    <li><a href="">Privacy</a></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

