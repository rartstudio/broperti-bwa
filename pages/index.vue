<template>
  <div>
    <div class="main">
        <div class="w-full bg-one min-h-screen max-h-screen h-screen relative">
          <HeaderParts/>
          <HeroParts/>
          <PassThrough class="top-0 absolute w-full transform scale-150 hidden md:block md:scale-100"/>
        </div>
        <ServicesParts/>
        <StatisticParts/>
        <div class="flex flex-col justify-start container mx-auto pb-64 px-4">
          <div class="flex justify-between items-center mb-12">
            <h2 class="text-xl md:text-2xl" data-aos="flip-left" data-aos-duration="500">You're Probably<br/>
              Gonna Love These
            </h2>
            <nuxt-link to="/home" class="text-sm text-right text-gray-600 underline inline-block" data-aos="flip-left" data-aos-duration="750">VIEW OTHER RECOMMENDATION</nuxt-link>
          </div>
          <ItemProperty/>
        </div>
    </div>
    <FooterParts/>
  </div>
</template>

<script>
import PassThrough from "~/assets/images/pass-through.svg?inline"
export default {
  components : {
    PassThrough
  }
}
</script>

<style>
.main {
  background: #F5F6F8;
}
.nuxt-link-active {
  @apply text-white;
}
.link:hover {
  @apply transition-all duration-200 text-white;
}
.main {
  font-family: 'Poppins';
}
.bg-one {
  background: #0F1837;
}
.bg-two {
  background: #83D987;
}
.bg-three {
  background: #E7E5F9;
}
.text-two {
  color: #0A9F82;
}
.text-three {
  color: #5943A6;
}
.top-20 {
  top:20px;
}
.-top-40 {
  top: -40px;
}
.right-230 {
  right: 230px;
}
.-bottom-134 {
  bottom: -134px;
}
.bottom-30 {
  bottom: 30px;
}
.left-60{
  left: 60px
}
.z-2 {
  z-index: 2;
}
.z-3 {
  z-index: 3;
}

</style>
