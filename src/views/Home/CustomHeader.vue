<template>
  <header class="header">
    <div class="header_group">
      <div class="flex items-center justify-between py-10">
        <div class="w-28 lg:w-36">
          <img class="w-full" src="@/assets/images/logo_white.png" alt="">
        </div>
        <div class="flex">
          <button class="px-6 py-2 font-bold text-white font-sans">Crie uma conta</button>
          <button class="px-6 py-2 font-sans text-brand-main font-bold bg-white rounded-full focus:outline-none">Entar</button>
        </div>
      </div>

      <div class="flex flex-col mt-28">
          <h1 class="text-4xl font-sans font-bold text-white">Tenha um feedback. <br>
          E faça seus clientes mais <br class="hidden lg:inline-block"/> felizes!</h1>
          <p class="text-white mt-5 text-lg font-sans font-medium">
            Receba ideias, reclamações e feedbacks com um<br class="hidden lg:inline-block"/>
            simples widget na página.
          </p>
          <div class="mt-10">
            <button class="px-6 py-2 font-sans text-brand-main font-bold bg-white rounded-full focus:outline-none">Crie uma conta grátis</button>
          </div>
      </div>

    </div>
  </header>
</template>

<script>
export default {
  setup () {
    return {}
  }
}
</script>

<style lang="postcss" scoped>
.header{
  @apply bg-brand-main w-full flex justify-center;
  height: 700px;
}

@media (min-width: 640px){
.header_group{
  @apply flex flex-col w-4/5 max-w-6xl;
  background-image: url(../../assets/images/balloon-blue.png);
  background-size: 628px;
  background-position: 90% 100%;
  background-repeat: no-repeat;
}

}

</style>
