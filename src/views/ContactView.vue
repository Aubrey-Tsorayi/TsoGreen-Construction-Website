<script setup>
import { ref, computed } from 'vue';

// Reactive state
const formData = ref({
  name: '',
  email: '',
  message: '',
});

// Computed properties
const isValidName = computed(() => formData.value.name.trim() !== '');
const isValidEmail = computed(() => {
  const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return emailRegex.test(formData.value.email);
});
const isValidMessage = computed(() => formData.value.message.trim() !== '');

// Methods
const submitForm = () => {
  if (isValidName.value && isValidEmail.value && isValidMessage.value) {
    // Form is valid, you can perform your submit logic here
    console.log('Form submitted:', formData.value);
  } else {
    // Form is not valid, you can handle validation errors here
    console.log('Form validation failed');
  }
};
</script>

<template>
  <div class="lg:grid lg:grid-cols-2 sm:grid-cols-1 items-center ml-4 mb-5">

    <div class="flex flex-col pt-5">
    <div class="flex justify-center animate-pulse">
      <h1 class="text-6xl lg:text-7xl font-bold font-title">TSO</h1>
      <h1 class="text-6xl lg:text-7xl font-bold text-green-500 font-title">GREEN</h1>
    </div>
    <div class="flex justify-center pt-2">
      <h1 class="lg:text-xl italic font-title">Let's build together...</h1>
    </div>
    </div>

    <div class="lg:min-h-screen flex items-center justify-center">
    <form @submit.prevent="submitForm" class="p-8 rounded shadow-lg">

      <div class="mb-4">
        <label for="name" class="block text-gray-700 text-sm font-bold mb-2">Name:</label>
        <input v-model="formData.name" type="text" id="name" name="name" placeholder="Enter your name"
               class="w-full p-2 border rounded" />
        <span v-if="!isValidName" class="text-red-500 text-sm">Name is required</span>
      </div>

      <div class="mb-4">
        <label for="email" class="block text-gray-700 text-sm font-bold mb-2">Email:</label>
        <input v-model="formData.email" type="email" id="email" name="email" placeholder="Enter your email"
               class="w-full p-2 border rounded" />
        <span v-if="!isValidEmail" class="text-red-500 text-sm">Please enter a valid email</span>
      </div>

      <div class="mb-6">
        <label for="message" class="block text-gray-700 text-sm font-bold mb-2">Message:</label>
        <textarea v-model="formData.message" id="message" name="message" rows="4"
                  placeholder="Type your message here" class="w-full p-2 border rounded"></textarea>
        <span v-if="!isValidMessage" class="text-red-500 text-sm">Message is required</span>
      </div>

      <button type="submit" class="bg-green-500 hover:bg-title text-white py-2 px-4 rounded flex items-center gap-2">Send a message<svg xmlns="http://www.w3.org/2000/svg"
                                                                                                                                   viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4">
        <path
            d="M2.87 2.298a.75.75 0 0 0-.812 1.021L3.39 6.624a1 1 0 0 0 .928.626H8.25a.75.75 0 0 1 0 1.5H4.318a1 1 0 0 0-.927.626l-1.333 3.305a.75.75 0 0 0 .811 1.022 24.89 24.89 0 0 0 11.668-5.115.75.75 0 0 0 0-1.175A24.89 24.89 0 0 0 2.869 2.298Z" />
      </svg>
      </button>
    </form>
    </div>
  </div>
</template>