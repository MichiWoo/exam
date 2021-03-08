<template>
  <form class="w-full">
    <div class="space-y-4">
      <TextInput
        name="email"
        type="email"
        label="Email"
        placeholder="Correo electrónico"
      />
      <TextInput
        name="password"
        type="password"
        label="Contraseña"
        placeholder="Contraseña"
      />
    </div>
    <div class="flex items-center justify-center w-full my-8">
      <BlockButton> Ingresar </BlockButton>
    </div>
    <div class="flex flex-col justify-around w-full sm:flex-row">
      <CheckInput name="keepSession" label="Mantenerme conectado" />
    </div>
    <div class="flex items-center justify-center">
      <p class="py-2 text-purple-700">
        También puedes iniciar sesión con tus redes
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
    <div class="flex flex-wrap mt-6">
      <div class="w-1/2">
        <a href="/" class="text-purple-700"
          ><small>¿Olvidaste la contraseña?</small></a
        >
      </div>
      <div class="w-1/2 text-right">
        <a href="/" class="text-purple-700"
          ><small>Crear una nueva cuenta</small></a
        >
      </div>
    </div>
  </form>
</template>

<script>
export default {
  name: 'Login',
  components: {
    BlockButton: () => import('@/components/buttons/BlockButton.vue'),
    IconButton: () => import('~/components/buttons/IconButton.vue'),
    TextInput: () => import('~/components/inputs/TextInput.vue'),
    CheckInput: () => import('~/components/inputs/CheckInput.vue'),
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
