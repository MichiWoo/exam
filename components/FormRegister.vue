<template>
  <form class="w-full">
    <div class="space-y-4">
      <TextInput
        name="nombre"
        type="text"
        label="nombre"
        placeholder="Nombre"
      />
      <TextInput
        name="email"
        type="email"
        label="Email"
        placeholder="Escriba su email"
      />
    </div>
    <div class="flex items-center justify-center w-full my-8">
      <BlockButton> Registrar </BlockButton>
    </div>
    <div class="flex items-center justify-center">
      <p class="py-2 text-purple-700">
        Ó también puedes registrarte con tus redes sociales
      </p>
    </div>
    <div class="flex items-center w-full justify-evenly">
      <IconButton>
        <Facebook class="w-4 h-4 mr-2" />
        <span>Facebook</span>
      </IconButton>
      <IconButton>
        <Google class="w-4 h-4 mr-2" />
        <span>Google</span>
      </IconButton>
    </div>
  </form>
</template>

<script>
export default {
  name: 'FormRegister',
  components: {
    BlockButton: () => import('@/components/buttons/BlockButton.vue'),
    IconButton: () => import('~/components/buttons/IconButton.vue'),
    TextInput: () => import('~/components/inputs/TextInput.vue'),
    Facebook: () => import('@/components/icons/Facebook'),
    Google: () => import('@/components/icons/Google'),
  },
  data() {
    return {
      email: '',
      password: '',
    }
  },
}
</script>
