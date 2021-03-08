<template>
  <nav
    class="absolute top-0 z-50 flex flex-wrap items-center justify-between w-full px-2 py-3 navbar-expand-lg"
  >
    <div
      class="container flex flex-wrap items-center justify-between px-4 mx-auto"
    >
      <div
        class="relative flex justify-between w-full lg:w-auto lg:static lg:block lg:justify-start"
      >
        <nuxt-link
          class="inline-block py-2 mr-4 text-sm font-bold leading-relaxed text-purple-700 uppercase whitespace-no-wrap"
          to="/"
          >Ex@m</nuxt-link
        ><button
          class="block px-3 py-1 text-xl leading-none bg-transparent border border-transparent border-solid rounded outline-none cursor-pointer lg:hidden focus:outline-none"
          type="button"
          @click="toggleNavbar()"
        >
          <Bars class="w-4 h-4 text-purple-700 fas fa-bars" />
        </button>
      </div>
      <div
        class="items-center flex-grow bg-purple-100 lg:flex lg:bg-transparent lg:shadow-none"
        :class="{ hidden: !showMenu, block: showMenu }"
      >
        <ul class="flex flex-col list-none lg:flex-row lg:ml-auto">
          <li class="flex items-center">
            <a
              class="flex items-center px-3 py-4 text-xs font-bold text-gray-800 uppercase lg:text-purple-700 lg:hover:text-purple-900 lg:py-2"
              href="#pablo"
            >
              <Share
                class="w-4 h-4 text-lg text-purple-500 lg:text-purple-700 leading-lg"
              />

              <span class="inline-block ml-2 lg:hidden">Share</span></a
            >
          </li>
          <li class="flex items-center">
            <a
              class="flex items-center px-3 py-4 text-xs font-bold text-gray-800 uppercase lg:text-purple-700 lg:hover:text-purple-300 lg:py-2"
              href="/"
            >
              <Twitter
                class="w-4 h-4 text-lg text-purple-500 lg:text-purple-700 leading-lg"
              />
              <span class="inline-block ml-2 lg:hidden">Tweet</span></a
            >
          </li>
          <li class="flex items-center">
            <nuxt-link to="/login">
              <Button
                class="text-white bg-purple-700 active:bg-purple-100 hover:bg-purple-400"
              >
                Login
              </Button>
            </nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  components: {
    Twitter: () => import('@/components/icons/Twitter'),
    Share: () => import('@/components/icons/Share'),
    Button: () => import('@/components/buttons/Button'),
    Bars: () => import('@/components/icons/Bars'),
  },
  data() {
    return {
      showMenu: false,
    }
  },
  methods: {
    toggleNavbar() {
      this.showMenu = !this.showMenu
    },
  },
}
</script>
