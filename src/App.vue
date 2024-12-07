<script setup lang="ts">
import Scroll from './components/Scroll.vue';
 

</script>

<template class="bg-[#12CFCF]" >
  <main class="  m-0">
    <div id="base" class="font-bold bg-[#e6f3fa] grid-cols-2 grid grid-rows-3   h-[100%]  text-4xl ">
      
        <div class="p-40">
        <p class="headerA mb-10"> Hi, my name is Patrick Emanuel Tomic. </p>
        <p class="text-2xl w-[30vw]">
        I'm an Independent Software Engineer Consultant from Tampa, Fl
        </p>
      </div>
        <img src="./assets/icon.jpg" alt="" class="w-[20vw] ml-40 mt-40  grid-rows-4 ">
      
      <div class="absolute top-[40%] left-[10%]">
        <p class="text-2xl p-40 ml-40">
         <span  v-bind:style ="{animationDelay: (0.5+0/10)+'s'}">S</span>
         <span v-bind:style ="{animationDelay: (0.5+1/10)+'s'}">C</span>
         <span v-bind:style ="{animationDelay: (0.5+2/10)+'s'}">R</span>
         <span v-bind:style ="{animationDelay: (0.5+3/10)+'s'}">O</span>
         <span v-bind:style ="{animationDelay: (0.5+4/10)+'s'}">L</span>
         <span v-bind:style ="{animationDelay: (0.5+5/10)+'s'}">L</span>
      </p></div>
     
      <div id="contact" class="text-3xl mt-[80vh] p-40">
      <p class="w-[40vw]">From single-page apps to cloud-based apps, starting from scratch, or rebuilding the brand. I help anyone needing assistance in the with web projects; whatever your imagination thinks,<b> I can build it</b>  </p>
   </div>
    </div>
  
  </main>
</template>

<style scoped lang="scss">
#base{
  span{
    bottom: -1em;
    opacity:0;
    animation: move-text .75s forwards;
    animation-delay:3s;
  }
  p{
    animation: opacity 1s;
    animation-iteration-count: 1;
    animation-timing-function: ease-in;
  }
  .headerA{
    width: 20vw;
  }
img{

  border-radius:5%;
  //bounce animation ***
  animation: user .3s;
    animation-direction: alternate;
    animation-iteration-count: 1;
}
   margin: 20px 20px;
  padding: 10px 10px;
}
@keyframes opacity {
  from{
    opacity: 0;
  }
  to{
    opacity: 1;
  }
  
}
@keyframes user{ ///source of bounce
  
    0%{ 
     
  transform: scale3d(0,0,0);

 
  }
 
    100%{
     
      transform: scale3d(1, 1, 1);
  
    
    }  

    
}
@keyframes move-text {
  0% {
    bottom: -0.2em;
    opacity: 1;
   
  }
  
  50% {
    bottom: 0.2em;
   
  }

  100% {
    bottom: 0;
    opacity: 1;
   
  }
}
@media (min-width: 1024px) {

  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

   
}
</style>
