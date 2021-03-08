<template>
  <form class="w-full">
    <div class="flex items-center justify-center">
      <p class="py-2 text-purple-700">
        Escribe tu email para recurerar tu contraseña
      </p>
    </div>
    <div class="space-y-4">
      <TextInput
        name="email"
        type="email"
        label="Email"
        placeholder="Correo electrónico"
      />
    </div>
    <div class="flex items-center justify-center w-full my-8">
      <BlockButton> Enviar </BlockButton>
    </div>
  </form>
</template>

<script>
export default {
  name: 'Recovery',
  components: {
    BlockButton: () => import('@/components/buttons/BlockButton.vue'),
    TextInput: () => import('~/components/inputs/TextInput.vue'),
  },
  data() {
    return {
      email: '',
    }
  },
}
</script>
