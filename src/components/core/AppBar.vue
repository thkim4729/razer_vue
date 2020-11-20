<template>
    <div class="app-bar">
        <v-app-bar absolute color="#111" dark height="100px">
            <v-spacer></v-spacer>
            <v-row class="gnb" justify="center" align="center" no-gutters>
                <router-link to="/">
                    <v-btn
                        text
                        class="logo"
                        :ripple="false"
                        id="no-background-hover"
                        @click="reload()"
                    >
                        <v-img
                            src="https://roundhillinvestments.com/assets/img/razer-logo.png"
                            max-width="200px"
                        ></v-img>
                    </v-btn>
                </router-link>
                <v-spacer></v-spacer>
                <v-btn text class="gnb_item" :ripple="false" id="no-background-hover"
                    >하드웨어</v-btn
                >
                <v-btn text class="gnb_item" :ripple="false" id="no-background-hover"
                    >소프트웨어</v-btn
                >
                <v-btn text class="gnb_item" :ripple="false" id="no-background-hover"
                    >커뮤니티</v-btn
                >
                <v-btn text class="gnb_item" :ripple="false" id="no-background-hover">스토어</v-btn>
                <v-btn text class="gnb_item" :ripple="false" id="no-background-hover"
                    >고객지원</v-btn
                >
                <v-btn icon class="gnb_item" :ripple="false" id="no-background-hover"
                    ><v-icon>mdi-magnify</v-icon></v-btn
                >
            </v-row>
            <v-spacer></v-spacer>
        </v-app-bar>
    </div>
</template>

<script>
export default {
    name: 'AppBar',
    data() {
        return {};
    },
    methods: {
        reload() {
            location.reload();
        },
    },
};
</script>

<style lang="scss" scoped>
.gnb_item {
    font-size: 16px;
    font-weight: 400;
    transition: all 0.2s;
}
.gnb_item:hover {
    color: #00ff00;
}
#no-background-hover::before {
    background-color: transparent !important;
}
</style>
