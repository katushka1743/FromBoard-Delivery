<script setup>

</script>


<template>
    <div class="content">
      <div class="hero">
        <div class="heroText">
          <p class="heroTextBold">Без проблемная доставка купленных вещей из США, Европы и Азии в Россию</p>
          <p class="heroTextSmall">Сэкономьте на покупках и наслаждайтесь мировыми брендами — наш сервис позволяет
            вам легко и удобно заказывать товары со всего мира и получать их в России</p>
          <img src="/src/img/Rectangle 2.png" alt="">
        </div>
        <div class="heroCalc">
          <div class="heroCalcText">
            <p class="heroCalcTextBold">Калькулятор доставки</p>
            <p class="heroCalcTextSmall">Посчитайте, сколько будет стоить перевозка покупки из зарубежа</p>
          </div>
          <form>
            <input type="text" name="" id="" placeholder="Имя">
            <div class="two">
              <input type="text" name="" id="" placeholder="Почта">
              <input type="text" name="" id="" placeholder="Телефон">
            </div>
            <div class="two">
              <input type="text" name="" id="" placeholder="Общая площадь, м²">
              <input type="text" name="" id="" placeholder="Вес, кг">
            </div>
            <div class="two">
              <input type="text" name="" id="" placeholder="Страна покупки">
              <input type="text" name="" id="" placeholder="Город покупки">
            </div>
            <div class="two">
              <input type="text" name="" id="" placeholder="Область доставки">
              <input type="text" name="" id="" placeholder="Город доставки">
            </div>

            <button class="order">Заказать расчёт</button>
          </form>
        </div>
      </div>
    </div>

</template>

<style scoped>


.hero {
  display: flex;
  flex-direction: row;
  gap: 24px;
  height: 584px;

}

.heroText {
  width: 756px;
  height: 584px;
}

.heroTextBold {
  font-family: 'FormularBlack';
  font-size: 36px;
  line-height: 40px;
  padding-bottom: 12px;
}

.heroTextSmall {
  font-size: 20px;
  line-height: 28px;
  padding-bottom: 16px;
}

.hero>img {
  width: 756px;
  height: 352px;
}

.heroCalc {
  display: flex;
  flex-direction: column;
  background-color: #F9FAFB;
  width: 756px;
  border-radius: 16px;
  padding: 24px 27px;
  align-items: center;
}

.heroCalcText {
  width: 358px;
  height: 100px;
  margin-bottom: 28px;
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.heroCalcTextBold {
  font-family: 'FormularBold';
  font-size: 30px;
  line-height: 36px;
}

.heroCalcTextSmall {
  font-family: 'Formular';
  line-height: 24px;
  width: 358px;
  height: 48px;
  text-align: center;
}

form {
  display: flex;
  flex-direction: column;
  gap: 24px;
  width: 496px;
}

input {
  border: 2px solid #111827;
  width: 493px;
  height: 45px;
  border-radius: 4px;
  /* font-family: 'FormularBold'; */
}

.two {
  display: flex;
  flex-direction: row;
  gap: 24px;
  width: 496px;
}

.two>input {
  width: 236px;
}

::-webkit-input-placeholder {
  padding-left: 12px;
  color: #9CA3AF;
}

.order {
  width: 496px;
  height: 44px;
  margin: 0;
}


</style>