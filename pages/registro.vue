<template>
  <div>
    <header>
      <Navbar />
    </header>
    <main>
      <div class="flex flex-col items-center justify-center mt-24">
        <div class="flex items-center justify-center w-3/6 lg:w-1/6">
          <Exam class="w-full" />
        </div>
        <h1 class="my-12 text-4xl font-bold text-gray-600">ex@m</h1>
        <div class="w-96 lg:w-2/6">
          <FormRegister />
        </div>
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'Registro',
  components: {
    FormRegister: () => import('@/components/FormRegister'),
  },
}
</script>
