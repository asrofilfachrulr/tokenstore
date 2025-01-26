<script setup>
import RootContainer from '~/components/RootContainer.vue'
import SimpleCard from '~/components/SimpleCard.vue'
import { ref } from 'vue'

const email = ref('')
const password = ref('')
</script>

<template>
  <RootContainer>
    <div class="max-h-full min-h-[1024px] w-full flex flex-col justify-center items-center gap-8">

      <h1 class="text-3xl font-semibold"><span class="text-accent">TokenStore</span> Login</h1>
      <SimpleCard :class="'w-full lg:w-[540px]'">
        <form>
          <div>
            <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Email</label>
            <input class="input-accent" id="email" required v-model="email" />
          </div>
          <div class="mt-8">
            <label for="password" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Password</label>
            <input class="input-accent" type="password" required v-model="password" />
          </div>
          <div class="mt-8 mb-4 flex justify-end gap-4">
            <a class="btn-accent-transparent" href="#">Register</a>
            <button class="btn-accent-primary float-end">Login</button>
          </div>
        </form>
      </SimpleCard>
    </div>
  </RootContainer>
</template>