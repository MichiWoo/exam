<template>
  <footer class="relative pt-8 pb-6 bg-gray-300">
    <div
      class="absolute top-0 left-0 right-0 bottom-auto w-full -mt-20 overflow-hidden pointer-events-none"
      style="height: 80px; transform: translateZ(0px)"
    >
      <svg
        class="absolute bottom-0 overflow-hidden"
        xmlns="http://www.w3.org/2000/svg"
        preserveAspectRatio="none"
        version="1.1"
        viewBox="0 0 2560 100"
        x="0"
        y="0"
      >
        <polygon
          class="text-gray-300 fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>
    <div class="container px-4 mx-auto">
      <div class="flex flex-wrap">
        <div class="w-full px-4 lg:w-6/12">
          <h4 class="text-3xl font-semibold">Escríbenos!</h4>
          <h5 class="mt-0 mb-2 text-lg text-gray-700">
            Nos puedes encontrar en cualquiera de nuestras redes sociales.
          </h5>
          <div class="mt-6">
            <SocialButton>
              <Twitter class="flex w-6 h-6" />
            </SocialButton>
            <SocialButton>
              <Facebook class="flex w-6 h-6" />
            </SocialButton>
          </div>
        </div>
        <div class="w-full px-4 my-6 lg:my-0 lg:w-6/12">
          <div class="flex flex-wrap mb-6 items-top">
            <div class="w-full px-4 ml-auto lg:w-4/12">
              <span
                class="block mb-2 text-sm font-semibold text-gray-600 uppercase"
                >Links de interés</span
              >
              <ul class="list-unstyled">
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://www.creative-tim.com/presentation"
                    >Acerca de</a
                  >
                </li>
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://blog.creative-tim.com"
                    >Blog</a
                  >
                </li>
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://www.creative-tim.com/bootstrap-themes/free"
                    >Precios</a
                  >
                </li>
              </ul>
            </div>
            <div class="w-full px-4 lg:w-4/12">
              <span
                class="block mb-2 text-sm font-semibold text-gray-600 uppercase"
                >Otros Recursos</span
              >
              <ul class="list-unstyled">
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://creative-tim.com/terms"
                    >Terms &amp; Conditions</a
                  >
                </li>
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://creative-tim.com/privacy"
                    >Privacy Policy</a
                  >
                </li>
                <li>
                  <a
                    class="block pb-2 text-sm font-semibold text-gray-700 hover:text-gray-900"
                    href="https://creative-tim.com/contact-us"
                    >Contact Us</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <hr class="my-6 border-gray-400" />
      <div
        class="flex flex-wrap items-center justify-center md:justify-between"
      >
        <div class="w-full px-4 mx-auto text-center md:w-4/12">
          <div class="py-1 text-sm font-semibold text-gray-600">
            Copyright © 2021
            <a
              href="https://www.creative-tim.com"
              class="text-gray-600 hover:text-gray-900"
              >WooLands Project</a
            >.
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  components: {
    SocialButton: () => import('@/components/buttons/SocialButton'),
    Facebook: () => import('@/components/icons/Facebook'),
    Twitter: () => import('@/components/icons/Twitter'),
  },
}
</script>
