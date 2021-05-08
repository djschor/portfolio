<template>
  <div>
    <section>
      <div>
        <div class="columns is-vcentered is-mobile">
          <div class="column is-9 is-centered content-block-wrap" style="margin-left: auto; margin-right: auto;">
            <div class="box content-block  is-one-half is-transparent" style="box-shadow:  39px 39px 83px #52b3ec, 
              -39px -39px 83px #58bffa;">
              <div class="vert-line"/>
              <h class="text-is-left is-h" >
              intro
              </h>
              <h2 class="text-is-left" style="color: #685206; font-family: 'Helvetica Neue', sans-serif; font-size: 16px; line-height: 24px; margin: 0 0 24px; text-align: justify; text-justify: inter-word;">
                Hi 👋 I'm <strong>Daniel</strong>. I'm a data scientist with over four years of experience (2 years full-time post graduate) implementing production level data science and software solutions. I specialize in full stack data science development across sectors, specifically predictive modeling, natural language processing (NLP), and cloud-driven ML-Ops. In my free time I love front-end development, any kind of physical activity especially running/basketball/skiing, and building my army of house plants 🌳
              </h2>
            </div>
            <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" >
              writing
              </h>
              <h2 class="text-is-left" >
              Musings data science, technology, and life with influences from various curiosities. 
              </h2>
              <blog-horizontal/>
            </div>
            <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" style="margin-bottom: 35px;">
              what i'm listening to
              </h>
              <music/>
            </div>
            <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" style="margin-bottom: 35px;">
              what i'm watching
              </h>
              <shows/>
            </div>
            <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" style="margin-bottom: 35px;">
              what i'm reading
              </h>
              <books
              />
            </div>
            <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" style="margin-bottom: 35px;">
              other interests
              </h>
              <interests
              />
            </div>
          </div>
        </div>
        

          <!-- <div class="box content-block  is-one-half is-transparent">
              <h class="text-is-left is-h" >
              what i'm listening to
              </h>

              <interest 
                image="~/assets/interests/pluto.png"
                title="Pluto x Baby Pluto"
                icon="icon-spotify"
              />
          </div> -->
        </div>
    </section>
  </div>  
</template>
<script>
import Card from '~/components/Card'
import PinkButton from '~/components/PinkButton'
import EmailButton from '~/components/EmailButton'
import PinkModal from '~/components/PinkModal'
import BlogHorizontal from '~/components/BlogHorizontal'
import Interest from '~/components/Interest'
import Music from '~/components/interests/Music'
import Shows from '~/components/interests/Shows'
import Books from '~/components/interests/Books'
import Interests from '~/components/interests/other'
import NuxtSSRScreenSize from 'nuxt-ssr-screen-size'

import { Icon } from 'ant-design-vue'
const MyIcon = Icon.createFromIconfontCN({
  scriptUrl: '//at.alicdn.com/t/font_2530486_df52i00yn3s.js', 
})
export default {
   name: 'HomePage',
   components: {
     Card,
     BlogHorizontal,
     PinkButton,
     Interest,
     Music,
     Shows,
     Books,
     Interests
   },
   head: {
    script: [
      { src: 'vanta/three.min.js' },
      { src: 'vanta/vanta.clouds.min.js' },
    ]
  },
  data() {
    return {
      isImageModalActive: false,
    }
  },
  mixins: [NuxtSSRScreenSize.NuxtSSRScreenSizeMixin],
  methods: {
    getWidth () {
      return this.$vssWidth
    }
  },
  async mounted() {
    // window is only avaiable on browser
    if (process.browser) {
      window.THREE = THREE;
      const { default: CLOUDS } = await import("@/static/vanta/vanta.clouds.min.js");
      VANTA.CLOUDS({
        el: "#section-background",
        mouseControls: true,
        touchControls: true,
        gyroControls: false,
        minHeight: 2200.00,
        minWidth: 800.00,
        cloudColor: 0xa4a4c0,
        sunColor: 0x98653f,
        speed: 0.10
      })
    }
  },
};
</script>
<style>
  @import url(https://fonts.googleapis.com/css?family=Khula:700);
  .title {
    font-family: 'Montserrat', sans-serif; 
    display: block;
    font-weight: 300;
    font-size: 67px;
    color: #35495e;
    letter-spacing: 1px;
    padding-bottom: 3px;
    padding-top: 20px;
    margin-bottom: 500px;

  }
  .title:hover { 
     color: #122f4e;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    /* padding-bottom: 5px; */
  }

  .title--kukuri {
    text-transform: uppercase;
    font-weight: 800;
    overflow: hidden;
    line-height: 0.75;
    color: #b2b0a9;
  }

  .title--kukuri:hover, .title--kukuri-mobile:hover {
    color: #122f4e;
  }
  .title--kukuri::after {
    display: absolute;
    content: '';
    position: absolute;
    height: 21px;
    width: 9.47em;
    top: 53.9%;
    margin-top: 1.55em;
    /* margin-left: auto; */
    background: #344c64;
    transform: translate3d(-100%,0,0);
    transition: transform 0.4s;
    transition-timing-function: cubic-bezier(0.7,0,0.3,1);
    opacity: 0.5;

  }
    .title--kukuri-mobile::after {
    content: '';
    position: absolute;
    height: 21px;
    width: 495px;
    top: 50.5%;
    /* margin-top: 95.5px; */
    margin-left: 0px;
    /* margin-right: 80px; */
    background: #344c64;
    transform: translate3d(-100%,0,0);
    transition: transform 0.4s;
    transition-timing-function: cubic-bezier(0.7,0,0.3,1);
    opacity: 0.5;

  }

  .title--kukuri:hover::after {
    transform: translate3d(100%,0,0);
  }

  .title--kukuri::before {
    content: attr(data-letters);
    position: absolute;
    z-index: 2;
    overflow: hidden;
    color: #424242;
    white-space: nowrap;
    width: 20%;
    transition: width 0.4s 0.3s;
  }

  .is-alt-section { 
    background-color:none 
  }


  body {
      filter: progid:DXImageTransform.Microsoft.gradient(gradientType=1, startColorstr='#faf7f0', endColorstr='#f0e1b9');
      background-size: 100%;
      background-image: -webkit-gradient(linear, 0 0, 100% 100%, color-stop(0, #faf8f3), color-stop(100%, #ffe395));      background-image: -moz-linear-gradient(45deg, #faf8f3, #f0e1b9);
      text-align: center;
      margin: 0px;
      overflow: hidden;
  }

.hidden {
  opacity:0;
}
/* .console-container {
 
  font-family:Khula;
  font-size:4em;
  text-align:center;
  height:200px;
  width:200px;
  display:block;
  position:absolute;
  color:white;
  top:0;
  bottom:0;
  left:0;
  right:0;
}
.console-underscore {
  display:'float';
  top:-0.14em;
  left:-100px;
} */
.line{
  margin: 0 auto;
  width: 73%;
  height: -40px;
  border-bottom: 1px solid black;
  position: relative;
  padding-left: 70px 0;
}
.bigger { 
  padding-bottom: 30px;
}
.has-margin-top { 
  margin-top: 20px;
}
.is-remove-top-margin { 
  margin-top: -20px;
}
.is-text { 
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 30;
  font-size: 20px;
  color: #35495e;
  letter-spacing: 0px;
  padding-bottom: 0px;
  padding-top: 20px;
}

.text-is-left { 
  text-align: left;
}
.is-top { 
  float: top;
}

.has-letter-spacing { 
  letter-spacing: 2px;
}
.is-transparent { 
  background-color: transparent;
}
.is-h {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: bold;
  font-size: 40px;
  color: #35495e;
  letter-spacing: -1px;
  padding-bottom: 0px;
  padding-top: 20px;
}
.icon-sm {
 width: 1em;
 height: 1em;
 fill: currentColor;
 vertical-align: -.125em;
 overflow: hidden;
}

.icony {
  width: 3em; height: 3em;
  vertical-align: -0.15em;
  fill: currentColor;
  overflow: hidden;
  margin-top: -11px;
 }
 
.is-left {
  float: left
}
.margin-left{
  margin-left: -100px;
}
.write-block { 
  border-radius: 25px;
  padding: 20px;
  width: 1200px;
  height: 80px;
  border: 2px solid rgb(84, 90, 114);
}
.is-higher { 
  margin-top: -11px;
}

.is-linky {
  position: relative;
  overflow: hidden;
  text-decoration: none;
  color: #344c64;
}
.is-linky::after {
  content: "";
  background: rgba(#344c64, 0.25);
  position: absolute;
  left: 12px;
  bottom: -6px;
  width: calc(100% - 8px);
  height: calc(100% - 8px);
  z-index: -1;
  transition: 0.35s cubic-bezier(0.25, 0.1, 0, 2.05);
}
.is-linky:hover::after {
  left: 0;
  bottom: -2px;
  width: 100%;
  height: 100%;
}
.is-linky-wrap {
  width: 50vw;
  box-sizing: border-box;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}
.is-lower{ 
  padding-top: 20px;
}

.content-block { 
  margin-left: auto; 
  margin-right: auto;
}
.content-block-wrap:hover .content-block{
  filter:blur(3px);
  opacity:.5;
  transform: scale(.98);
  box-shadow:none;
  
}
.content-block-wrap:hover .content-block:hover{
  transform:scale(1);
  filter:blur(0px);
  opacity:1;
  box-shadow:0 8px 20px 0px rgba(0,0,0,0.125);
  border-left: 20px solid #8AA8A1;
}


</style>
