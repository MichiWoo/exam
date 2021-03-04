<template>
  <div class="container mx-auto">
    <div class="flex flex-col items-center justify-center my-48">
      <Logo />
      <h1 class="my-12 text-4xl font-bold text-gray-600">ex@m</h1>
      <div class="pt-8">
        <a
          href="https://app.asana.com/0/1199987690132502/overview"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 mx-2 border-2 border-green-300 rounded-md"
        >
          Documentación Proyecto
        </a>
        <a
          href="https://github.com/MichiWoo/exam.git"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 mx-2 border-2 border-gray-600 rounded-md"
        >
          GitHub Proyecto.
        </a>
      </div>
      <div
        class="flex items-center justify-center w-4/6 py-8 my-8 rounded-xl sm:w-2/6"
      >
        <nuxt-link to="/login">Login</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
