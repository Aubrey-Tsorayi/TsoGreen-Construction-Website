<script setup>

</script>

<template>


<footer class="bg-green-500 font-title">
    <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-5">
        <div class="md:flex md:justify-between">
          <div class="mb-6 md:mb-0">
              <a href="/" class="flex items-center">
                  <img src="../assets/logo.jpg" class="h-8 me-3" alt="TsoGreen Logo" />
                  <span class="self-center text-2xl font-semibold whitespace-nowrap">TSOGREEN</span>
              </a>
          </div>
          <div class="">
              <div class="flex items-center lg:items-start lg:flex-row">
                  <ul class="flex flex-col space-y-6 lg:space-y-0 lg:space-x-6 lg:flex-row ml-3">
                    <RouterLink to="/" class="hover:text-white hover:cursor-pointer font-title">Home</RouterLink>
                    <RouterLink to="/about" class="hover:text-white hover:cursor-pointer font-title truncate">About Us</RouterLink>
                    <RouterLink to="/services" class="hover:text-white hover:cursor-pointer font-title truncate">Services</RouterLink>
                    <RouterLink to="/contact" class="hover:text-white hover:cursor-pointer font-title truncate">Get a Qoute</RouterLink>
                  </ul>
              </div>
          </div>
        </div>
      <hr class="my-6 border-black-200 sm:mx-auto lg:my-4" />
      <div class="sm:flex sm:items-center sm:justify-between">
          <span class="text-sm text-black sm:text-center ">© 2024 <a href="/" class="hover:underline">TsoGreen Construction™</a>. All Rights Reserved.
          </span>
          <div class="flex mt-4 sm:justify-center sm:mt-0">
              <a href="#" class="text-black  hover:text-white">
                  <svg class="w-4 h-4" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 8 19">
                        <path fill-rule="evenodd" d="M6.135 3H8V0H6.135a4.147 4.147 0 0 0-4.142 4.142V6H0v3h2v9.938h3V9h2.021l.592-3H5V3.591A.6.6 0 0 1 5.592 3h.543Z" clip-rule="evenodd"/>
                    </svg>
                  <span class="sr-only">Facebook page</span>
              </a>
              <a href="#" class="text-black hover:text-white ms-5">
                  <svg class="w-4 h-4" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 17">
                    <path fill-rule="evenodd" d="M20 1.892a8.178 8.178 0 0 1-2.355.635 4.074 4.074 0 0 0 1.8-2.235 8.344 8.344 0 0 1-2.605.98A4.13 4.13 0 0 0 13.85 0a4.068 4.068 0 0 0-4.1 4.038 4 4 0 0 0 .105.919A11.705 11.705 0 0 1 1.4.734a4.006 4.006 0 0 0 1.268 5.392 4.165 4.165 0 0 1-1.859-.5v.05A4.057 4.057 0 0 0 4.1 9.635a4.19 4.19 0 0 1-1.856.07 4.108 4.108 0 0 0 3.831 2.807A8.36 8.36 0 0 1 0 14.184 11.732 11.732 0 0 0 6.291 16 11.502 11.502 0 0 0 17.964 4.5c0-.177 0-.35-.012-.523A8.143 8.143 0 0 0 20 1.892Z" clip-rule="evenodd"/>
                </svg>
                  <span class="sr-only">Twitter page</span>
              </a>
          </div>
      </div>
    </div>
</footer>

</template>

<style lang="scss" scoped></style>