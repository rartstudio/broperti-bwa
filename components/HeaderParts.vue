<template>
    <header class="flex px-4 md:px-0 justify-between items-center pt-8 container mx-auto">
            <img src="~assets/images/logo.png" alt="">
            <ul class="hidden md:flex items-center justify-center text-gray-600">
              <li>
                <nuxt-link to="/" class="mx-4 link">Home</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/home" class="mx-4 link">Featured</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/home" class="mx-4 link">Stories</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/home" class="mx-4 link">Partner</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/home" class="mx-4 link">About</nuxt-link>
              </li>
            </ul>
            <nuxt-link to="/home" class="hidden md:block px-4 py-2 bg-two rounded-lg">
              My Account
            </nuxt-link>
          </header>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>