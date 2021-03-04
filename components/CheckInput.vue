<template>
  <div class="flex flex-col justify-center flex-start">
    <label
      class="flex items-center justify-between text-purple-700"
      :for="name"
    >
      <span>{{ label }}</span>
      <input
        :id="name"
        v-model="inputValue"
        type="checkbox"
        :name="name"
        class="border-purple-700 border-1"
      />
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
