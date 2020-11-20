<template>
    <footer>
        <div class="inner">
            <v-row class="footer_menu" justify="center" no-gutters>
                <v-col class="footer_item">
                    <dt>Our Network</dt>
                    <dd>Razer.com</dd>
                    <dd>Razer Gold & Silver</dd>
                    <dd>Razer Pay</dd>
                    <dd>Game Deals</dd>
                </v-col>
                <v-col class="footer_item">
                    <dt>Shop</dt>
                    <dd>Razer Store (Online)</dd>
                    <dd>Razer Store (Retail)</dd>
                    <dd>Store Locator</dd>
                    <dd>My Account</dd>
                    <dd>Newsletter</dd>
                    <dd>Affiliate</dd>
                </v-col>
                <v-col class="footer_item">
                    <dt>Software/Services</dt>
                    <dd>Razer ID</dd>
                    <dd>Synapse 3</dd>
                    <dd>Chroma</dd>
                    <dd>Cortex</dd>
                    <dd>Developer Portal</dd>
                </v-col>
                <v-col class="footer_item">
                    <dt>Company</dt>
                    <dd>About Razer</dd>
                    <dd>Press Room</dd>
                    <dd>Investor Relations</dd>
                    <dd>Careers</dd>
                    <dd>zVentures</dd>
                </v-col>
                <v-col class="footer_item">
                    <dt>Need Help?</dt>
                    <dd>Support</dd>
                    <dd>Warranty</dd>
                    <dd>Contact Us</dd>
                </v-col>
                <v-col class="footer_item">
                    <dt>Connect</dt>
                    <dd>Get Started</dd>
                    <dd>Insider</dd>
                    <dd>
                        <v-btn icon color="#777">
                            <v-icon>mdi-facebook</v-icon>
                        </v-btn>
                    </dd>
                    <dd>
                        <v-btn icon color="#777">
                            <v-icon>mdi-twitter</v-icon>
                        </v-btn>
                    </dd>
                    <dd>
                        <v-btn icon color="#777">
                            <v-icon>mdi-instagram</v-icon>
                        </v-btn>
                    </dd>
                </v-col>
            </v-row>
            <!--footer_menu-->
            <p class="copyright">
                Copyright © 2020 Razer Inc. All rights reserved. | Legal Terms | Privacy Policy |
                Cookie Policy
            </p>
        </div>
        <!--inner-->
    </footer>
</template>

<script>
export default {
    name: 'Footer',
};
</script>

<style lang="scss" scoped>
.inner {
    width: 1200px;
    margin: 0 auto;
}
footer {
    margin-top: 100px;
}

.footer_menu {
    text-align: center;
    display: flex;
    flex-flow: row;
    /* border: 1px solid red; */
}

.footer_menu .footer_item {
    text-align: left;
    width: 10%;
    margin-right: 7.8%;
    /* border: 1px solid blue; */
}

.footer_menu .footer_item:last-child {
    margin-right: 0;
}

.footer_menu .footer_item dt {
    color: white;
    font-size: 16px;
    margin-bottom: 5px;
    font-weight: bold;
}

.footer_menu .footer_item dd {
    color: #777;
    font-size: 14px;
    transition: all 0.3s;
    text-decoration: none;
    padding: 5px 0;
    cursor: pointer;
}

.footer_menu .footer_item dd:hover {
    color: #00ff00;
}

.copyright {
    margin-top: 50px;
    font-size: 12px;
    color: #777;
    text-align: center;
}
</style>
