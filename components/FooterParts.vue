<template>
    <footer class="bg-white flex flex-col items-center justify-center" data-aos="slide-up" data-aos-duration="500">
      <div class="w-full flex items-center justify-center px-4 md:px-0">
        <form class="form-register w-full md:w-7/12 pr-4 bg-one flex flex-col md:flex-row justify-between p-4 pl-4 mt-12 rounded-lg relative z-10">
          <div class="w-full mt-8 md:mt-0 md:w-4/12 flex flex-col justify-start">
            <label class="text-white">Full Name</label>
            <input class="px-4 py-2 bg-gray-200 md:w-64" type="text" value="Masayoshi Haza"/>
          </div>
          <div class="w-full mt-8 md:mt-0 md:w-4/12 flex flex-col justify-start">
            <label class="text-white">Email Address</label>
            <input class="px-4 py-2 bg-gray-200 md:w-64" type="text" value="masayoshi@bwa.co.id"/>
          </div>
          <div class="w-full mt-8 md:mt-0 md:w-3/12">
            <button class="px-8 py-5 bg-two rounded-lg ml-auto hover:shadow-lg w-full">Sign Up</button>
          </div>
        </form>
      </div>
      <p class="text-center px-4 text-gray-600 -mt-16">Copyright 2021. All Rights Reserved Pixel by BuildWith Angga and Coded by Rudi.</p>
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style>
@media (max-width:640px){
    .form-register {
        transform : translateY(-200px);
    }
}
@media (min-width:768px){
    .form-register {
        transform : translateY(-100px);
    }
}
</style>