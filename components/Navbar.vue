<template>
    <header>
        <v-container class="wrapper">
            <div class="title">
                <h2>Krunal</h2>
            </div>

            <div class="social-links">
                <v-btn class="links" color="#dfe6e9" href="https://www.linkedin.com/in/krunalsagathiya/" icon link outlined rounded>
                    <v-icon>mdi-linkedin</v-icon>
                </v-btn>
                <v-btn class="links mx-4" color="#dfe6e9" href="mailto:krunal_sagathiya@hotmail.co.uk" icon link outlined rounded>
                    <v-icon>mdi-email</v-icon>
                </v-btn>
                <v-btn class="links" color="#dfe6e9" href="https://github.com/digvijay-webdev" icon link outlined rounded>
                    <v-icon>mdi-github</v-icon>
                </v-btn>
            </div>
        </v-container>
    </header>
</template>

<script>
export default {
    name: "Navbar"
}
</script>

<style scoped>
header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 10;
    padding: 8px 0;
    background: #121212b5;
    box-shadow: 0 4px 30px #0000001a;
    backdrop-filter: blur(4px);
    -webkit-backdrop-filter: blur(5px);
    border: 1px solid #4e4e4e7f;
}

.wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.social-links .links {
    padding: 6px;
}
</style>
