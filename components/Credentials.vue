<template>
    <div class="main">
        <v-container>
            <h1>Licenses & certifications</h1>
            <v-list color="transparent" three-line>
                <v-list-item data-aos="fade-up" v-for="item in list" :key="item.id">
                    <v-list-item-avatar>
                        <v-img :src="item.imgURL"></v-img>
                    </v-list-item-avatar>
                    <v-list-item-content>
                        <v-list-item-title>{{ item.title }}</v-list-item-title>
                        <v-list-item-subtitle>{{ item.subtitle }}</v-list-item-subtitle>
                    </v-list-item-content>
                    <v-list-item-action>
                        <v-btn large :href="item.credURL" link icon>
                            <v-icon color="blue lighten-1">mdi-eye</v-icon>
                        </v-btn>
                    </v-list-item-action>
                </v-list-item>
            </v-list>
        </v-container>
    </div>
</template>

<script>
import aosMixin from "@/mixin/aos.js";

export default {
    name: "Credentials",
    mixins: [aosMixin],
    data() {
        return {
            list: [
                {
                    id: 1,
                    title: "Watson and Cloud Foundations",
                    subtitle: "IBM, Issued Apr 2022",
                    imgURL: "https://media.licdn.com/dms/image/C560BAQE9wp87-KDfwg/company-logo_100_100/0/1657054972290?e=1683763200&v=beta&t=n34ZZcP388UHnciDUMX5fcjTG3kBPsCePjKAOLFiTak",
                    credURL: "https://www.credly.com/badges/81389098-6dad-4618-91fa-faa9ed7e86c0?source=linked_in_profile"
                },
                {
                    id: 2,
                    title: "IBM Cloud Pak for Data V3.5.x Data Engineer",
                    subtitle: "IBM, Issued Nov 2021",
                    imgURL: "https://media.licdn.com/dms/image/C560BAQE9wp87-KDfwg/company-logo_100_100/0/1657054972290?e=1683763200&v=beta&t=n34ZZcP388UHnciDUMX5fcjTG3kBPsCePjKAOLFiTak",
                    credURL: "https://www.credly.com/badges/cbf7a16c-277f-44ba-91a7-995212cfe955?source=linked_in_profile"
                },
            ]
        }
    }
}
</script>

<style scoped>
.main {
    border-bottom: 1px solid #4e4e4e7f;
}

.container {
    border-right: 1px solid #4e4e4e7f;
}
</style>
