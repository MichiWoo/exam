<template>
  <div>
    <Header />
    <main>
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
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {
    Header: () => import('@/components/Header'),
    Footer: () => import('@/components/Footer'),
  },
}
</script>
