<template>
  <div
    class="flex items-center justify-center w-2/6 py-2 mx-2 my-2 text-white bg-purple-700 rounded-full hover:bg-purple-900 focus:outline-none focus:ring-2 focus:ring-offset-purple-700 focus:ring-opacity-50"
  >
    <div class="flex items-center justify-center">
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  name: 'SocialButton',
}
</script>
