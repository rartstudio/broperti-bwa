<template>
    <header class="flex px-4 md:px-0 justify-between items-center pt-8 container mx-auto">
      <div :class="[ToggleMenu ? 'fixed z-50 -mx-4 px-4 pt-18' : '','flex justify-between w-full md:w-3/12 items-center']">
            <img src="~assets/images/logo.png" class="z-50" alt="">
            <div class="flex md:hidden">
                <button @click="setToggleMenu(ToggleMenu)"
                    :class="['toggle z-50', ToggleMenu ? 'active' : '']"
                    >
                </button>
            </div>
      </div>
            <ul :class="['fixed inset-0 bg-gray-900 md:bg-transparent md:relative md:opacity-100 md:visible pt-24 md:pt-0 transition-all duration-200  overflow-hidden md:flex items-center justify-center text-gray-600',ToggleMenu ? 'opacity-100 visible z-40' : 'opacity-0 invisible']">
              <li class="my-4 md:my-0">
                <nuxt-link to="/" class="mx-4 link">Home</nuxt-link>
              </li>
              <li class="my-4 md:my-0">
                <nuxt-link to="/home" class="mx-4 link">Featured</nuxt-link>
              </li>
              <li class="my-4 md:my-0">
                <nuxt-link to="/home" class="mx-4 link">Stories</nuxt-link>
              </li>
              <li class="my-4 md:my-0">
                <nuxt-link to="/home" class="mx-4 link">Partner</nuxt-link>
              </li>
              <li class="my-4 md:my-0">
                <nuxt-link to="/home" class="mx-4 link">About</nuxt-link>
              </li>
              <li class="my-8 md:my-0">
                <nuxt-link to="/home" class="md:block mx-4 px-4 py-2 text-white bg-two rounded-lg">
                  My Account
                </nuxt-link>
              </li>
            </ul>
          </header>
</template>

<script>
    export default {
        data() {
          return {
            ToggleMenu: false
          }
        },
        methods: {
            setToggleMenu(toggle){
                return this.ToggleMenu = !toggle
            }
        },
    }
</script>

<style>
.pt-18 {
  padding-top: 60px;
}
.toggle {
    position: relative;
    width: 20px;
    height: 20px;
    z-index: 9999;
}
.toggle:focus {
    outline: none
}
.toggle:before,
.toggle:after{
    @apply right-0 absolute bg-gray-200 transition-all duration-200;
    content: "";
    height:3px;
    transform-origin:center;
}
.toggle:before{
    top:26%;
    width: 20px;
}
.toggle:after{
    top: 58%;
    width: 12px;
}
.toggle.active:before{
    transform: translateY(-50%) rotate(-45deg);
}
.toggle.active:after{
    transform: translateY(-50%) rotate(45deg);
}
.toggle.active:before, .toggle.active:after {
    width: 20px;
    top: 50%;
}
</style>