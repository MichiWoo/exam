<template>
  <div
    class="flex flex-col-reverse items-center justify-center w-full h-screen lg:flex-row"
  >
    <div
      class="flex items-center justify-center w-full bg-purple-200 h-14 lg:h-full lg:w-1/6"
    >
      Sidebar
    </div>
    <div
      class="flex items-center justify-center w-full h-full bg-gray-100 lg:h-full lg:w-5/6"
    >
      Contenido
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>
