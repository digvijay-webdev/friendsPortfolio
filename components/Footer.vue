<template>
    <div class="main mt-2">
        <v-footer padless>
            <v-card flat tile width="100%" color="#121212" class="text-center">
                <v-card-text>
                    <v-btn link href="https://www.linkedin.com/in/krunalsagathiya/" class="mx-4" icon>
                        <v-icon size="24px">mdi-linkedin</v-icon>
                    </v-btn>
                    <v-btn link href="mailto:krunal_sagathiya@hotmail.co.uk" class="mx-4" icon>
                        <v-icon size="24px">mdi-email</v-icon>
                    </v-btn>
                    <v-btn link href="https://github.com/KrunalSagathiya" class="mx-4" icon>
                        <v-icon size="24px">mdi-github</v-icon>
                    </v-btn>
                </v-card-text>

                <v-card-text class="white--text">
                {{ new Date().getFullYear() }} — Designed & Developed By <strong><a href="https://digvijay.tech">Digvijay Padhiyar</a></strong>
                </v-card-text>
            </v-card>
        </v-footer>
    </div>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>
a {
    outline: none;
    text-decoration: none;
    color: #0984e3;
}
</style>
