<template>
  <div>
    <header>
      <Navbar />
    </header>
    <main>
      <div class="flex flex-col items-center justify-center my-20 lg:my-48">
        <div class="flex items-center justify-center w-3/6 lg:w-1/6">
          <Exam class="w-full" />
        </div>
        <h1 class="my-12 text-4xl font-bold text-gray-600">ex@m</h1>
        <div class="flex flex-wrap pt-8">
          <a
            href="https://app.asana.com/0/1199987690132502/overview"
            target="_blank"
            rel="noopener noreferrer"
            class="p-2 mx-2 border-2 border-purple-300 rounded-md"
          >
            Documentación Proyecto
          </a>
          <a
            href="https://github.com/Woolands"
            target="_blank"
            rel="noopener noreferrer"
            class="p-2 mx-2 border-2 border-gray-600 rounded-md"
          >
            GitHub Organización.
          </a>
        </div>
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {
    Navbar: () => import('@/components/Navbar'),
    Footer: () => import('@/components/Footer'),
  },
}
</script>
