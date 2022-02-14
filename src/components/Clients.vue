<template>
    <!-- clients -->
      <div id="clients" class="clients ">
         <div class="container">
            <div class="row">
               <div class="col-md-12">
                  <div class="titlepage">
                     <h2>Our Clients</h2>
                     <p> A reader will be distracted by the readable content of a page when looking at its layout. The point of using LoremIt is a </p>
                  </div>
               </div>
            </div>
            <div class="row d_flex">
               <div class="col-md-10 offset-col-md-1">
                  <div id="myCarousel" class="carousel slide clients_slider" data-ride="carousel">
                     <!-- <ol class="carousel-indicators">
                        <li data-target="#myCarousel" data-slide-to="0" class=""></li>
                        <li data-target="#myCarousel" data-slide-to="1" class="active"></li>
                        <li data-target="#myCarousel" data-slide-to="2" class=""></li>
                     </ol> -->
                     <div class="carousel-inner">
                        <carousel :autoplay="true" :loop="true" :perPage="1" :pagenation="true">
                           <slide v-for="(client,key) in clients" :key="key">
                        <div class="carousel-item active">
                           <div class="container">
                              <div class="carousel-caption">
                                 <div class="row d_flex">
                                    <div class="col-xl-5 col-lg-5 col-md-5 col-sm-12 pa_rile">
                                       <div class="img_box">
                                          <i><img src="../assets/images/icon_1.png" alt="#"></i>
                                          <figure><img :src="require(`@/assets/images/${client.imgPath}`)" alt="blog image"></figure>
                                       </div>
                                    </div>
                                    <div class="col-xl-7 col-lg-7 col-md-7 col-sm-12 pa_rile">
                                       <div class="joe">
                                          <h3>{{client.name}}</h3>
                                          <p>{{client.desc}}</p>
                                       </div>
                                    </div>
                                 </div>
                              </div>
                           </div>
                        </div>
                           </slide>
                        </carousel>
                     </div>
                     <a class="carousel-control-prev" href="#myCarousel" role="button" data-slide="prev">
                     <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                     <span class="sr-only">Previous</span>
                     </a>
                     <a class="carousel-control-next" href="#myCarousel" role="button" data-slide="next">
                     <span class="carousel-control-next-icon" aria-hidden="true"></span>
                     <span class="sr-only">Next</span>
                     </a>
                  </div>
               </div>
            </div>
         </div>
      </div>
      <!-- end clients -->
</template>
<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  components: {
    Carousel,
    Slide,
  },
  data () {
     return {
        clients:[
           {
              name:"Joi",
              desc:"It is a long established fact that a reader will be distracted",
              imgPath:"clients.png"
           },
           {
              name:"Joi",
              desc:"It is a long established fact that a reader will be dist",
              imgPath:"clients.png"
           },
           {
              name:"Joi",
              desc:"It is a long established fact that a reader will be distracted",
              imgPath:"clients.png"
           },
        ]
     }
  }
}
</script>
<style scoped>

</style>