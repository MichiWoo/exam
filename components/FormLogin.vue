<template>
  <form class="w-2/6">
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
      <router-link to="/recover-password" class="text-purple-700"
        >¿Olvidaste la contraseña?</router-link
      >
      <CheckInput name="keepSession" label="Mantenerme conectado" />
    </div>
    <div class="flex items-center justify-center">
      <p class="py-2">También puedes iniciar sesión con tus redes</p>
    </div>
    <div class="flex items-center w-full justify-evenly">
      <SocialButton>
        <Facebook class="w-8 h-8" />
      </SocialButton>
      <SocialButton>
        <Google class="w-8 h-8" />
      </SocialButton>
    </div>
  </form>
</template>

<script>
export default {
  name: 'Login',
  components: {
    BlockButton: () => import('@/components/buttons/BlockButton.vue'),
    SocialButton: () => import('@/components/SocialButton.vue'),
    TextInput: () => import('~/components/inputs/TextInput.vue'),
    CheckInput: () => import('@/components/CheckInput.vue'),
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
