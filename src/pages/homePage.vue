<template>
  <q-page class="bg-blue-grey-9">
    <!-- content -->
    <div class="row bg-blue-grey-13" style="height: 350px;">
       <div class="col ">
        <div style="text-align: center;" class="q-ma-lg " >
          <div class="text-h4 text-white text-bold q-mt-lg q-pt-lg">Learn Quasar for improve your UI design in faster way  </div>
        <div class="text-6 text-light-blue-4 q-px-lg q-py-lg q-pb-sm">Here you can search for video</div>
        
        <q-input class="bg-blue-grey-1 rounded-borders  q-mb-lg " filled v-model="text" :dense="dense" >
          <template v-slot:append>
            <div class="text-cyan-6">
              <q-icon v-if="text !== ''" name="close" @click="text = ''" class="cursor-pointer" />
              <q-icon  name="search" />
        </div>
        </template>

        </q-input>

        </div>
       </div>

       <div class="col q-ma-xl gt-sm">
        
        <q-img style="height: 250px;" src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*8k4KGgByJl2bbAXKGJCBUA.png" :ratio="16/9">
          <div class="absolute-bottom text-subtitle1 text-center">
            
          </div>
        </q-img>
       </div>
    </div>

    <!--content2-->
    <div class="bg-blue-grey q-my-sm text-center q-py-sm shadow-2 text-bold text-cyan-11 text-h6">
      Tutorial
    </div>
    
     <!--content3-->
     <div class="row">
      <!--video1-->
      <div class="col-12 col-md">
        <div class="q-pa-md">
       <q-card class="my-card">
           <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

          <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
           </q-card-section>

           <q-card-section class="q-pt-none">
               Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
               eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
    </q-card>
  </div>
      </div>
      

  <!--video2-->
  <div class="col-12 col-md">
        <div class="q-pa-md">
       <q-card class="my-card">
           <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

          <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
           </q-card-section>

           <q-card-section class="q-pt-none">
               Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
               eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
    </q-card>
  </div>
  </div>

  <!--video3-->
  <div class="col-12 col-md">
        <div class="q-pa-md">
       <q-card class="my-card">
           <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

          <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
           </q-card-section>

           <q-card-section class="q-pt-none">
               Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
               eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
    </q-card>
  </div>
  </div>
  <!--video4-->
  <div class="col-12 col-md">
        <div class="q-pa-md">
       <q-card class="my-card">
           <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

          <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
           </q-card-section>

           <q-card-section class="q-pt-none">
               Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
               eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
    </q-card>
  </div>
  </div>
  <!--finish-->
  <q-footer bordered class="bg-blue-11 shadow-2 ">
        <q-tabs no-caps active-color="primary" indicator-color="transparent" class="text-black" v-model="tab">
          <q-tab name="images" label="Images" />
          <q-tab name="videos" label="Videos" />
          <q-tab name="articles" label="Articles" />
        </q-tabs>
      </q-footer>
     </div>
     
  <!---->
 </q-page>
</template>

<script>
import { ref } from 'vue'
export default {
  // name: 'PageName',
  setup () {
    return {
      text: ref(''),
      ph: ref(''),
      dense: ref(false)
    }
  }
}
</script>
