<script setup>

</script>

<template>

  <!-- <body> -->
    <div class="content">
      <div class="headerBenefits">Наши преимущества</div>
      <div class="benefitsPoints">
        <div class="benefitPoint">
          <img src="/src/img/Board.png" alt="">
          <div class="text">
            <p class="textBold">Растоможка груза</p>
            <p class="textSmall">Мы берём на себя все формальности и бумажную волокиту, связанную с растаможкой груза
            </p>
          </div>
        </div>
        <div class="benefitPoint">
          <img src="/src/img/Package.png" alt="">
          <div class="text">
            <p class="textBold">Надёжная упаковка</p>
            <p class="textSmall">Все товары упаковываются нашими специалистами с особым вниманием к деталям, гарантируя,
              что они дойдут
              в безопасности и в отличном состоянии</p>
          </div>
        </div>
        <div class="benefitPoint">
          <img src="/src/img/Delivery.png" alt="">
          <div class="text">
            <p class="textBold">Быстро и выгодно</p>
            <p class="textSmall">Мы предлагаем быструю и выгодную доставку, чтобы вы могли насладиться покупками как можно
              скорее.</p>
          </div>
        </div>


        <div class="benefitPoint">
          <img src="/src/img/best support.png" alt="">
          <div class="text">
            <p class="textBold">Удобный сервис</p>
            <p class="textSmall">Стремимся сделать процесс доставки максимально удобным для вас, чтобы опыт остался
              приятным и беззаботным
            </p>
          </div>
        </div>

        <div class="benefitPoint">
          <img src="/src/img/clear info.png" alt="">
          <div class="text">
            <p class="textBold">Прозрачность работы</p>
            <p class="textSmall">Мы предоставляем полный контроль над каждым этапом доставки, от момента заказа до момента
              прибытия заказа
            </p>
          </div>
        </div>

        <div class="benefitPoint">
          <img src="/src/img/garantee.png" alt="">
          <div class="text">
            <p class="textBold">Страхование груза</p>
            <p class="textSmall">Наше страхование обеспечивает полную защиту и покрытие почти все неприятные и неожиданные
              ситуации</p>
          </div>
        </div>
      </div>
    </div>

  <!-- </body> -->
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 24px;
  /* padding-bottom: 72px; */
}

.headerBenefits {
  font-family: 'FormularBlack';
  font-size: 30px;
  line-height: 36px;
}

img {
  width: 136px;
  height: 136px;
}

.benefitsPoints {
  display: flex;
  flex-wrap: wrap;
  gap: 24px;
}

.benefitPoint {
  display: flex;
  flex: 1 1 calc(33.333% - 20px);
  /* flex: 1 1 33%; */
  gap: 12px;
  align-items: center;
}

.text {
  display: flex;
  flex-direction: column;
  width: 300px;
  gap: 12px;
}

.textBold {
  font-size: 24px;
  line-height: 32px;
  font-family: 'FormularBlack';
}

.textSmall {
  font-size: 14px;
  line-height: 20px;
}
</style>