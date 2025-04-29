<script setup lang="ts">
 var currentdate = new Date(); 
 var datetime = currentdate.getDate() + "/"
  + (currentdate.getMonth()+1)  + "/" 
  + currentdate.getFullYear() + " - "  
  + currentdate.getHours() + ":"  
  + currentdate.getMinutes() + ":" 
  + currentdate.getSeconds();
</script>

<template>
 <div class="container">
  <header>
   <p class="text--large">
    {{ datetime }}
   </p>
   <h1 class="title--large">
    Aogosto's Pub
   </h1>
  </header>
  <hr>
  <main>
   <div class="title">
    <h3 class="title--small">
    Monday, April 28, 2025
    </h3>
    <h6 class="text--large">
     18:29 [Bus] 1001 Musics, Day 0001 - Vol. 4 (Black Sabbath)
    </h6>
   </div>
   <div class="text">
    <img src="https://i.scdn.co/image/ab67616d0000b273f44c5014a32565b63475d7b2" alt="Vol. 4 (Black Sabbath) Cover">
   </div>
  </main>
 </div>
</template>

<style scoped lang="scss">
 * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: georgia, 'times new roman', times,serif;
 }
 .container {
  max-width: 960px;
  width: 100%;
  margin: 0 auto;
  padding: 10px;
 }
 hr {
  margin: 10px 0;
 }
 .title {
  margin: 10px 0;
 }
 img {
  border: 1px solid white;
 }
 @mixin title($font-size: 40px) {
  @include text($font-size);
  color: white;
 }
 @mixin text($font-size: 16px) {
  font-size: $font-size;
  line-height: $font-size + 10px;
  color: silver;
 }
 .title--large {
  @include title(44px);
  @media (max-width: 768px) {
   @include title(26px);
  }
 }
 .title--medium {
  @include title;
  @media (max-width: 768px) {
   @include title(24px);
  }
 }
 .title--small {
  @include title(28px);
  @media (max-width: 768px) {
   @include title(22px);
  }
 }
 .text--large {
  @include text(18px);
  @media (max-width: 768px) {
   @include text(15px);
  }
 }
 .text--medium {
  @include text;
  @media (max-width: 768px) {
   @include text(14px);
  }
 }
 .text--small {
  color: silver;
  @include text(12px);
  @media (max-width: 768px) {
   @include title(11px);
  }
 }
 .link {
  @include text;
  color: white;
  text-decoration: underline;
 }
</style>
