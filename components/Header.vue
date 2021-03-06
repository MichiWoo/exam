<template>
  <header>
    <p>Header</p>
  </header>
</template>

<script>
export default {
  name: 'Header',
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
