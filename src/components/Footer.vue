<template>
    <div class="footer">
        <div class="logo-section">
            <Logo logoTextColor="white" logoBackgroundColor="white" logoCircleTextColor="#5B9BF3"/>
            <div class="text spacing">Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone</div>
            <div class="text">©Trafalgar PTY LTD 2020. All rights reserved</div>
        </div>
        <div class="d-flex footer-links">
            <FooterLinks v-for="(link, index) in links" :key="index" :link="link"/>
        </div>
    </div>
</template>

<script>
    import Logo from "./Logo.vue"
    import FooterLinks from "./FooterLinks.vue"

    export default {
        data() {
            return {
                links: [
                    {title: "Company", 
                    links:["About", "Testimonials", "Find a Doctor", "Apps"]},
                    {title: "Region", 
                    links:["Indonesia", "Singapore", "HongKong", "Canada"]},
                    {title: "Help", 
                    links:["Help Center", "Contact Support", "Instructions", "How it works"]}
                ],
            }
        },
        components: {
            Logo,
            FooterLinks
        },
    }
</script>

<style lang="scss" scoped>
    .footer {
        width: 100%;
        background: linear-gradient(183.41deg, #67C3F3 -8.57%, #5A98F2 82.96%);
        left: 0;
        bottom: 0;
        padding: 118px 120px 113px 190px ;  
        display: flex;  
        flex-direction: row;
        align-items: center;

        @media (max-width: 480px) {
            flex-direction: column;
            padding: 50px 24px;
        }
    }
    .logo-section {
        width: 391px;
        flex-direction: column;
        margin-right: 145px;

        
        @media (max-width:480px) {
            width: unset;
            margin-right: 0;
        }
    }
    .text {
        font-weight: 300;
        font-size: 18px;
        line-height: 28px;
        color: #FFFFFF;
    }
    .spacing {
        margin-top: 17px;
        margin-bottom: 31px;
    }
    .footer-links {
        
    @media (max-width:480px) {
        flex-direction: column;
        width: 100%;
        margin-top: 36px  }
    }
</style>