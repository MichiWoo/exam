<template>
  <div class="flex flex-col justify-center w-full flex-start">
    <label class="text-purple-700" :for="name">{{ label }}</label>
    <input
      :id="name"
      v-model="inputValue"
      class="w-full text-purple-700 bg-purple-100 border-purple-700 rounded shadow-xl border-1 focus:outline-none focus:ring-2 focus:border-transparent focus:ring-purple-700 focus:ring-offset-purple-700"
      :name="name"
      :type="type"
      :placeholder="placeholder"
    />
    <div
      v-show="errorMessage"
      class="flex items-center justify-start w-full mt-1"
    >
      <span v-show="errorMessage" class="text-red-700">
        {{ errorMessage }}
      </span>
    </div>
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
    value: {
      type: String,
      default: '',
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
  data() {
    return {
      errorMessage: '',
      inputValue: '',
    }
  },
}
</script>
