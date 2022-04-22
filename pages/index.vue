<template>
  <div class="main-page">
    <Header></Header>
    <main class="main">
      <div class="container">

      </div>
    </main>
  </div>
</template>

<script>
export default {
  layout: 'default',
  components: {
    Header: () => import('~/components/Header.vue'),

  }
}
</script>

<style>
.container{
  width: 95%;
  margin: auto;
}
</style>

