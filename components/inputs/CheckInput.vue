<template>
  <div class="flex flex-col justify-center flex-start">
    <label
      class="flex items-center justify-between text-purple-700"
      :for="name"
    >
      <div class="flex items-center justify-center">
        <span class="mr-2 font-semibold form-checkbox">{{ label }}</span>
        <input
          :id="name"
          v-model="inputValue"
          type="checkbox"
          :name="name"
          class="w-5 h-5 text-purple-700 border-2 border-purple-700 checked:bg-purple-700 checked:border-transparent"
          style="transition: all 0.15s ease 0s"
        />
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
