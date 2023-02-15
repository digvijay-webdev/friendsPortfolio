<template>
    <div class="main">
        <!-- <img id="circle" src="/circle.png" alt=""> -->
        <v-container class="container">
            <div class="wrapper">
                <div class="image-section">
                    <div class="frame">
                        <img src="https://media.licdn.com/dms/image/C4D03AQGDXjC4WZIIlQ/profile-displayphoto-shrink_400_400/0/1517252671243?e=1681344000&v=beta&t=BaJ9zVzSoRyAz5uK_h3nSn8uFv0jvWJdg1uXePP-G7o" alt="">
                    </div>
                </div>
                <div class="content-section">
                    <h1>Hello 👋 I'm Krunal,</h1>
                    <h3>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima rerum tenetur pariatur est.</h3>
                    <p>
                        Krunal Sagathiya is a Data Engineer Senior Manager at PWC. He has overall 13+ years of experience with expertise in Data Modelling, Analytics, Stakeholder Management, practical and innovative design solutions across Finance, Banking & Public sector. Krunal possesses strong problem solving, analytics and technical skills. Krunal has a first-class Master’s degree In Professional Computing from Leeds Metropolitan University.
                    </p>
                    <div>
                        <a href="https://www.linkedin.com/in/krunalsagathiya/">Let's connect</a>
                    </div>
                </div>
            </div>
        </v-container>
    </div>
</template>

<script>
export default {
    name: "Hero"
}
</script>

<style scoped>
.main {
    margin-top: 80px;
    border-bottom: 1px solid #4e4e4e7f;
}
.container {
    border-left: 1px solid #4e4e4e7f;
}
.wrapper {
    height: 80vh;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-content: center;
}

.wrapper .content-section, .wrapper .image-section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}

.wrapper .content-section, .wrapper .image-section img {
    border-radius: 4px;
}

.wrapper .image-section img {
    /* background: linear-gradient(235deg, #0088ff, #060b20, #89ff00); */
    /* position: relative; */
}
/* .wrapper .image-section img::before {
    content: "";
    position: absolute;
    left: -2px;
    top: -2px;
    right: -2px;
    bottom: -2px;
    background: #fff;
    z-index: -1;
} */
/* .wrapper .image-section img::after {
    content: "";
  position: absolute;
  left: -2px;
  top: -2px;
  right: -2px;
  bottom: -2px;
  background: #fff;
  z-index: -2;
  filter: blur(40px);
}

.wrapper .image-section img::before, .wrapper .image-section img::after {
  background: linear-gradient(235deg, #0088ff, #060b20, #89ff00);
} */

.content-section {
    padding-left: 18px;
}

.content-section h1 {
    font-size: 44px;
}

.content-section h3 {
    font-size: 22px;
    color: #d1dadd;
}

.content-section p {
    color: #b2bec3;
}

.content-section div {
    width: max-content;
    margin-bottom: 12px;
}

.content-section div a {
    outline: none;
    color: #fff;
    text-decoration: none;
    transition: all .3s ease;
}
.content-section div a::after {
    content: "";
    width: 60%;
    height: 1px;
    background: #fff;
    display: block;
    transition: all .3s ease;
}
.content-section div a:hover::after {
    width: 0;
}

/* circle animation */
/* #circle {
    animation: Hue 2s alternate infinite;
}

@keyframes Hue {
    to {
        filter: hue-rotate(1turn);
    }
} */

/* media quesries */
@media screen and (max-width: 940px) {
    .wrapper {
        height: max-content;
        display: flex;
        flex-direction: column;
    }
    .wrapper .image-section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 32px;
    }
    .wrapper .image-section img {
        border-radius: 100%;
        width: 250px;
    }
}
</style>
