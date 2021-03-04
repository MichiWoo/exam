<template>
  <div class="container mx-auto">
    <div class="flex flex-col items-center justify-center my-48">
      <Logo />
      <h1 class="my-12 text-4xl font-bold text-gray-600">ex@m</h1>
      <div class="pt-8">
        <a
          href="https://app.asana.com/0/1199987690132502/overview"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 mx-2 border-2 border-green-300 rounded-md"
        >
          Documentación Proyecto
        </a>
        <a
          href="https://github.com/MichiWoo/exam.git"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 mx-2 border-2 border-gray-600 rounded-md"
        >
          GitHub Proyecto.
        </a>
      </div>
      <div
        class="flex items-center justify-center w-4/6 py-8 my-8 bg-purple-100 rounded-xl sm:w-2/6"
      >
        <form class="w-5/6">
          <TextInput
            name="email"
            type="email"
            label="Email"
            placeholder="email@domain.com"
          />
          <div class="flex items-center justify-center w-full my-8">
            <CheckInput name="check" label="Da click" />
          </div>
          <div class="flex items-center justify-center w-full my-8">
            <ButtonBlock>Enviar</ButtonBlock>
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
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
    TextInput: () => import('@/components/TextInput'),
    ButtonBlock: () => import('@/components/ButtonBlock'),
    SocialButton: () => import('@/components/SocialButton'),
    Facebook: () => import('@/components/icons/Facebook'),
    Google: () => import('@/components/icons/Google'),
    CheckInput: () => import('@/components/CheckInput'),
  },
}
</script>
