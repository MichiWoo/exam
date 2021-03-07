<template>
  <div class="container mx-auto">
    <div class="flex flex-col items-center justify-center mt-24">
      <div class="flex items-center justify-center w-3/6 lg:w-1/6">
        <Exam class="w-full" />
      </div>
      <h1 class="my-12 text-4xl font-bold text-gray-600">ex@m</h1>
      <div
        class="flex items-center justify-center w-4/6 py-2 my-2 rounded-xl sm:w-2/6"
      >
        <nuxt-link to="/">Regresar</nuxt-link>
      </div>
      <FormLogin />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Login',
  components: {
    FormLogin: () => import('@/components/FormLogin'),
  },
}
</script>
