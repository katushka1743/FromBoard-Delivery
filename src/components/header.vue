<script setup>


</script>

<template>
  <header>
    <d>
      <div class="up">
        <div class="divLogo">
          <img src="/src/img/Frame 2.png" alt="">
        </div>
        <div class="upInfo">
          <div class="upInfoOne">
            <p>Доставляем товары из заграницы в Россию</p>
            <p>Стоимость от 550 рублей за заказ</p>
            <p>1 $ = 93 ₽ | 1 € = 99 ₽ | 1 ¥ = 13 ₽</p>
          </div>
          <img class="vector" src="/src/img/Vector 1.png" alt="">
          <div class="upInfoTwo">
            <p class="upInfoTwoPhone">+7 (800) 123 45-67</p>
            <p class="upInfoTwoText">Звонки по России бесплатны</p>
          </div>
        </div>
      </div>
      <div class="down">
        <nav>
          <button class="navBtn"><a href="#" class="calc">Калькулятор</a></button>
          <button class="navBtn"><a href="#">О нас</a></button>
          <button class="navBtn"><a href="#">Гарантии</a></button>
          <button class="navBtn"><a href="#">Отзывы</a></button>
        </nav>
        <button class="order">Оставить заявку</button>
      </div>
    </d>
  </header>

</template>

<style scoped>
header {
  display: flex;
  flex-direction: column;
  gap: 24px;
  height: 192px;

}

.up {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  font-size: 16px;
  gap: 515px;
  width: 1536px;
  margin-top: 24px;

}

.divLogo {
  width: 305px;
  height: 74px;
  margin: 0;
  padding: 0;
}

.divLogo img {
  width: 305px;
  height: 74px;
  margin: 0;
  padding: 0;
}

.upInfo {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  /* line-height: 0.5; */
  height: 76px;
  width: 716px;
}

.vector {
  padding-inline: 12px;
  width: 1px;
}

.upInfoOne {
  min-width: 349px;
  text-align: end;
}

.upInfoOne>p {
  height: 24px;
}

.upInfoTwo {
  width: 343px;
}

.upInfoTwoPhone {
  font-size: 36px;
  max-height: 40px;
  width: 341px;
  font-family: 'FormularBlack';
}

.upInfoTwoText {
  font-size: 24px;
  width: 343px; 
  height: 32px;
  font-family: 'FormularLight';
}

.down {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  /* margin-bottom: 24px; */
  margin-block: 24px;
}

nav {
  display: flex;
  flex-direction: row;
  width: 372px;
  height: 24px;
  justify-content: space-between;
  gap: 24px;
  padding: 0;
}

.navBtn {
  font-family: 'FormularBold';
  /* background-color: #F9FAFB;  */
  background-color: white;
  padding: 0;
}

.navBtn > a {
  font-family: 'FormularBold';
  /* font-family: ''; */
}

.navBtn> a:hover {
  color: #8B5CF6;
}

.calc {
  color: #8B5CF6;
  border-bottom: 2px dashed #8B5CF6;
}

.order {
  width: 196px;
  height: 44px;
}

</style>
