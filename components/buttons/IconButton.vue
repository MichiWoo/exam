<template>
  <button
    class="inline-flex items-center px-4 py-2 mb-1 mr-2 text-xs font-bold text-purple-800 uppercase bg-white rounded shadow outline-none active:bg-purple-100 focus:outline-none hover:shadow-md"
    type="button"
    style="transition: all 0.15s ease 0s"
  >
    <slot />
  </button>
</template>

<script>
export default {
  name: 'IconButton',
}
</script>
