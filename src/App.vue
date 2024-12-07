<script setup lang="ts">
 
</script>

<template class="bg-[#12CFCF]" >
  <main class=" h-[100vh] m-0">
    <div id="header" class="font-bold bg-[#e9fcf2]   h-[100%]  text-4xl flex items-center justify-around ">
      <div>
        <p class="headerA mb-10"> Hi, my name is Patrick Emanuel Tomic. </p>
        <p class="text-2xl w-[30vw]">
          I am a Software Engineer building Applications ranging from Landing Pages to Full Stack Applications. 
        </p>
      </div>
     
      <img src="./assets/icon.jpg" alt="" class="w-[20vw]">
    </div>
   
  </main>
</template>

<style scoped lang="scss">
#header{
  .headerA{
    width: 20vw;
  }
img{
  border-radius:5%;
  //bounce animation ***
  animation: user 0.5s;
    animation-direction: alternate;
    animation-iteration-count: 2;
}
   margin: 20px 20px;
  padding: 10px 10px;
}
@keyframes user{ ///source of bounce
  from { transform: translate3d(0, 0, 0);
 
  }
    to { transform: translate3d(-100px, 100px, 0);
    
    
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
