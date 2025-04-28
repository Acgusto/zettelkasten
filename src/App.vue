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
   <p class="text--small">
    {{ datetime }}
   </p>
   <h1 class="title--large">
    Aogosto's Pub
   </h1>
  </header>
  <hr>
  <main>
   <div class="date_and_time">
    <h3 class="title--small">
    Sunday, April 27, 2025
    </h3>
    <h6 class="text--large">
     22:33
    </h6>
   </div>
   <p class="text--medium">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae ducimus beatae nobis sed voluptates fuga magni doloremque, fugit sunt perspiciatis nulla corrupti aspernatur dignissimos quas aliquid, quod ratione, quos dolorem! Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quisquam quidem dolorem dolor! Nisi velit autem corporis eos praesentium nostrum dignissimos doloribus animi, magnam tempore libero molestias, ut obcaecati odio recusandae? Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minima inventore voluptas sapiente hic, et vel eligendi distinctio, dignissimos maxime dolorem facilis libero architecto quos tenetur possimus, maiores vitae non cumque! Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam non sunt maiores porro ea provident alias odio at fuga doloremque, praesentium quae! Animi quidem magni accusantium delectus ipsam, exercitationem quasi! Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cumque, sequi nulla praesentium aperiam doloribus reprehenderit cum numquam fugit, iusto, velit sint enim dolor possimus et architecto natus minima recusandae quos. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Mollitia dolorum adipisci facere molestias, beatae fugit quia corrupti recusandae vitae assumenda et eveniet aut pariatur eum enim! Vero quidem voluptate quam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Omnis fuga dicta magnam cupiditate libero, officiis explicabo natus vero? Quam natus nulla at tenetur quisquam similique molestias. Doloribus explicabo aspernatur hic! Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laborum cumque, in placeat molestiae velit, nostrum neque eum quis eaque dolore voluptates possimus debitis ut dolor sint tempore nulla. Rerum, exercitationem. Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque quibusdam fuga laboriosam? Fuga hic recusandae odio iusto maiores a impedit debitis, vero modi voluptate officiis, sed laborum dicta, dolorem eos?
   </p>
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
 .date_and_time {
  margin: 10px 0;
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
