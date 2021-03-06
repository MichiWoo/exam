<template>
  <button
    class="items-center justify-center w-10 h-10 p-2 mr-2 font-normal text-blue-400 bg-white rounded-full shadow-lg outline-none align-center focus:outline-none"
  >
    <slot />
  </button>
</template>

<script>
export default {
  name: 'SocialButton',
}
</script>
