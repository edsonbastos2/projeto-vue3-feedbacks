<template>
  <custom-header
    @create-account="handleAccountCreate"
    @login="handleLogin"
  />
  <contact/>
  <div class="flex justify-center py-10 bg-brand-gray">
    <p class="font-sans font-bold text-center text-gray-800">feedback © 2021</p>
  </div>
</template>

<script>
import CustomHeader from './CustomHeader.vue'
import Contact from './Contact.vue'
import { useRouter } from 'vue-router'
export default {
  components: {
    CustomHeader,
    Contact
  },
  setup () {
    const router = useRouter()
    const token = window.localStorage.getItem('token')
    if (token) {
      router.push({ name: 'Feedbacks' })
    }

    function handleLogin () {}
    function handleAccountCreate () {}
    return {
      handleLogin,
      handleAccountCreate
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
