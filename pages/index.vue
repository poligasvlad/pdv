<template>
  <div class="main-page">
    <Header></Header>
    <main class="main">
      <div class="container">
        <div class="wrapper">
          <h1>
            Оцінка A? - Тоді Вам на As’ hub.<br>
            Попіклуємось про ваші дедлайни самі!
          </h1>
          <p>
            Вітаємо на As’ hub!<br>
            Ми ті, хто допоможе Вам покращити успішність в школі, університеті та інших навчальних закладах.<br>
            Реферати, статті, курсові роботи, презентації та інші роботи, які виконають за тебе.<br>
            Оформлюйте своє замовлення прямо зараз та отримайте якісну роботу, відповідно до встановлених Вами дедлайнами.<br>
          </p>
          <div class="btn-wrapper">
            <button class="btn">Замовити роботу</button>
            <button class="btn">Стати автором</button>
          </div>
        </div>
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
@import '~/assets/styles/pages/index.scss';
</style>

