<template>
  <div class="relative w-full mb-3">
    <label
      class="block mb-2 text-xs font-bold text-purple-700 uppercase"
      :for="name"
      >{{ label }}</label
    ><input
      :type="type"
      class="w-full px-3 py-3 text-sm text-purple-700 placeholder-purple-400 bg-white rounded shadow focus:outline-none focus:ring-2 focus:border-transparent focus:ring-purple-700 focus:ring-offset-purple-700"
      :name="name"
      :placeholder="placeholder"
      style="transition: all 0.15s ease 0s"
    />
  </div>
</template>

<script>
export default {
  name: 'TextInput',
  props: {
    type: {
      type: String,
      default: 'text',
    },
    name: {
      type: String,
      required: true,
    },
    label: {
      type: String,
      required: true,
    },
    placeholder: {
      type: String,
      default: '',
    },
  },
}
</script>
