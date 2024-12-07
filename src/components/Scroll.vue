<script setup lang="ts">
  const arr = ['S','C','R','O','L','L']
 
</script>
<template>
<span v-for="(letter, index) in arr"  style="animation-delay: (0.5+index/10)+{${`s`}};">{{ letter }}</span>
</template>

<style>
</style>