<template>
  <div class="flex flex-col justify-center flex-start">
    <label
      class="flex items-center justify-between text-purple-700"
      :for="name"
    >
      <div class="flex items-center justify-center">
        <span class="mr-2">{{ label }}</span>
        <input
          :id="name"
          v-model="inputValue"
          type="checkbox"
          :name="name"
          class="text-purple-700 rounded"
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
