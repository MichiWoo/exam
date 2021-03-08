<template>
  <div class="flex flex-col justify-center flex-start">
    <label class="flex items-start justify-start">
      <div class="mr-2 text-purple-700">{{ label }}</div>
      <div
        class="flex items-center justify-center flex-shrink-0 w-6 h-6 mr-2 bg-white border-2 border-purple-700 rounded focus-within:border-purple-500"
      >
        <input
          :id="name"
          v-model="inputValue"
          type="checkbox"
          :name="name"
          class="absolute opacity-0"
          style="transition: all 0.15s ease 0s"
        />
        <svg
          class="hidden w-4 h-4 text-purple-700 pointer-events-none fill-current"
          viewBox="0 0 20 20"
        >
          <path d="M0 11l2-2 5 5L18 3l2 2L7 18z" />
        </svg>
      </div>
    </label>
  </div>
</template>

<script>
export default {
  name: 'CheckInput',
  props: {
    name: {
      type: String,
      default: '',
    },
    label: {
      type: String,
      default: '',
    },
  },
  data() {
    return {
      inputValue: true,
    }
  },
}
</script>

<style scoped>
input:checked + svg {
  display: block;
}
</style>
