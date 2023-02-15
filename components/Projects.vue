<template>
    <div class="main">
        <v-container class="container">
            <h1 class="mb-2">Projects</h1>

            <v-card data-aos="fade-up" color="transparent" v-for="item in list" :key="item.id">
                <v-row>
                    <v-col cols="12" sm="12" md="6" lg="4">
                        <v-img :src="item.imgURL"></v-img>
                    </v-col>
                    <v-col cols="12" sm="12" md="6" lg="8">
                        <v-card-title>{{ item.title }}</v-card-title>
                        <v-card-text>
                            {{ item.body }}
                        </v-card-text>
                    </v-col>
                </v-row>
            </v-card>
        </v-container>
    </div>
</template>

<script>
import aosMixin from "@/mixin/aos.js";

export default {
    name: "Projects",
    mixins: [aosMixin],
    data() {
        return {
            list: [
                {
                    id: 1,
                    imgURL: "https://media.licdn.com/media/AAYQAQQSAAgAAQAAAAAAACKYFNB5zdTqTlavWXkK0XvX-A.jpg",
                    title: "Project Title | 2022",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse rerum soluta velit voluptatibus, obcaecati reprehenderit maiores facere asperiores quam laborum cumque consectetur vitae minima placeat, odio ratione nisi tempora ea eligendi itaque!"
                },
                {
                    id: 2,
                    imgURL: "https://media.licdn.com/media/AAYQAQQSAAgAAQAAAAAAACKYFNB5zdTqTlavWXkK0XvX-A.jpg",
                    title: "Project Title | 2022",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse rerum soluta velit voluptatibus, obcaecati reprehenderit maiores facere asperiores quam laborum cumque consectetur vitae minima placeat, odio ratione nisi tempora ea eligendi itaque!"
                },
                {
                    id: 3,
                    imgURL: "https://media.licdn.com/media/AAYQAQQSAAgAAQAAAAAAACKYFNB5zdTqTlavWXkK0XvX-A.jpg",
                    title: "Project Title | 2022",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse rerum soluta velit voluptatibus, obcaecati reprehenderit maiores facere asperiores quam laborum cumque consectetur vitae minima placeat, odio ratione nisi tempora ea eligendi itaque!"
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
    border-left: 1px solid #4e4e4e7f;
}
</style>
