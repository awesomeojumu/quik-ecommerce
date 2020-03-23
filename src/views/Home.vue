<template>
  <div class="home">
    <div class="container-md"> 
      <div class="bannercontrol">
        <Banner v-for="link in banners" :catban="link" :key="link.id"/>
      </div>
    </div>
    <div>
        <div class="fixed-top">
            <Navbar />
        </div>
    </div>
      <div class="container">
        <div class="row position-static" >
          <div class="col-3">
            <div>
              <div>
                <Sidebar/>
              </div>
            </div>
          </div>
          <div class="col-9">
            <div>
              <div>
                <Carouselbar style="background-color:blue;"/>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="container">
          <div class="row align-items-start">
            <div class="row">
                <Tradetray v-for="comodity in comodities" :product="comodity" :key="comodity.id" />
          </div>
      </div>
      </div>
      <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue'
import Navbar from '@/components/Navbar.vue'
import Sidebar from '@/components/Sidebar.vue'
import Carouselbar from '@/components/Carouselbar.vue'
import Tradetray from '@/components/Tradetray.vue'
import Footer from '@/components/Footer.vue'
import { Carousel, Slide } from 'vue-carousel';

export default {
    name: 'Home',
      components: {
      Banner,
      Navbar,
      Sidebar,
      Carouselbar,
      Carousel,
      Slide,
      Tradetray,
      Footer
    },
    data(){
        return{
          banners: 
            [
              {
                bn:'a',
                links: 'Food'
              },
              {
                bn:'b',
                links: 'Gadgets'
              }, 
              {
                bn:'c',
                links: 'Housing'
              }, 
              {
                bn:'d',
                links:'Travels'
              },
              {
                bn:'e',
                links: 'Suprises'
              },
              {
                bn:'f',
                links: 'Real time'
              }
            ],
            comodities : 
            [ 
              {
                id : 1,
                name : "Traditional turn stick",
                price : "4,000",
                imageLink : require("@/assets/photos/tdturn.jpg")
              },
              {
                id : 2,
                name : "3 in 1 Throw Pillow",
                price : "5,000",
                imageLink : require("@/assets/photos/3throw2.jpg")
              },
              {
                id : 10,
                name : "NBA 2k20",
                price : "7,000",
                 imageLink : require('../assets/photos/nba2k20.jpg')
              },
              {
                id : 3,
                name : "4/6 Hard Bed",
                price : "12,000",
                imageLink : require("@/assets/photos/foam.jpg")
              },
              {
                id : 4,
                name : "Microwave",
                price : "15,000",
                imageLink : require("@/assets/photos/mwave.jpg")
              },
              {
                id : 5,
                name : "Pulpit",
                price : "15,000",
                imageLink : require("@/assets/photos/pulpit.jpg")
              },
              {
                id : 6,
                name : "Kitchen Towel",
                price : "5,000",
                imageLink : require("@/assets/photos/kittowel.jpg")
              },
              {
                id : 7,
                name : "3 in 1 Throw pillow",
                price : "5,000",
                imageLink : require("@/assets/photos/3throw.jpg")
              },
              {
                id : 8,
                name : "Standard Fridge",
                price : "40,000",
                imageLink : require("@/assets/photos/fridge.jpg")
              },
              {
                id : 9,
                name : "Microwave",
                price : "15,000",
                imageLink : require("@/assets/photos/mwave.jpg")
              },{
                id : 11,
                name : "Microwave",
                price : "15,000",
                imageLink : require("@/assets/photos/mwave.jpg")
              },{
                id : 12,
                name : "Microwave",
                price : "15,000",
                imageLink : require("@/assets/photos/mwave.jpg")
              },
            ]
        }
      }
}
</script>

<style>
  .bannercontrol{
    padding-left:100px;
    padding-right: 100px;
  }
</style>
