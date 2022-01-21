<template>
    <v-container>
        <div id="component-profile" class="d-flex flex-column justify-center align-center">
            <img 
            src="https://scontent.fldb1-1.fna.fbcdn.net/v/t1.6435-9/174547508_3737544919682482_3411299680349001008_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=09cbfe&_nc_eui2=AeFP8-qqTvE-NOZd3RymTgIoqPI9CTjBVk-o8j0JOMFWT0fE6wod_mAxyIZg68ev7_kN2YpPzIjWEX3LxJC1PisJ&_nc_ohc=mkSmQKM-LtoAX82ceoU&_nc_ht=scontent.fldb1-1.fna&oh=00_AT-fNMzo3gBk-I1r0hcJStc_Dcb0OnbBwfEu7ArPOQMZGg&oe=620E108D"
            alt="Rafael Paduan" />
            <h1>{{ name }}</h1>
            <p v-html="description"></p>
            <div class="v-flex">
                <a :href="github" target="_blank"><i class="fab fa-github mx-2"></i></a>
                <a :href="linkedin" target="_blank"><i class="fab fa-linkedin mx-2"></i></a>
                <a :href="'https://api.whatsapp.com/send?phone=' + whatsapp" target="_blank"><i class="fab fa-whatsapp mx-2"></i></a>
                <a :href="'mailto:' + email" target="_blank"><i class="fas fa-at mx-2"></i></a>
            </div>
        </div>
    </v-container>
</template>

<script>

export default {

    components: {
        
    },

    data() {
        return {
            name: "Rafael Paduan",
            description: "Administrador de Sistemas,<br>desenvolvedor PHP e NodeJS<br>e pai de três lindas meninas",
            
            github: "https://github.com/rafaelpaduan",
            linkedin: "https://www.linkedin.com/in/rafael-a-paduan-santos-530802a8/",
            email: "rafaelpaduan2013@gmail.com",
            whatsapp: "5543999745305"
        }
    }
}

</script>

<style scoped lang="scss">

#component-profile {

    height: 100vh;
    img {
        max-height: 100px;
        border-radius: 100px;
    }
    p {
        text-align: center;
    }

    i {
        font-size: 24px;
        color: darkred;
    }
}

</style>