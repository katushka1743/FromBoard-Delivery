<script setup></script>

<template>
  <div class="contentFooter">

    <div class="Frame38">
      <div class="Frame2">
        <img src="/src/img/Frame 1.png" alt="">
        <div class="pImg">
          <p class="smallTextImg">2025 © Разработкой сайта в учебных целях занималась katushka1743</p>
          <!-- <img src="/src/img/Vector5.png" alt=""> -->
        </div>
      </div>

      <div class="Frame7">
        <nav>
          <button class="navBtn"><a href="#" class="calc">Калькулятор</a></button>
          <button class="navBtn"><a href="#">О нас</a></button>
          <button class="navBtn"><a href="#">Гарантии</a></button>
          <button class="navBtn"><a href="#">Отзывы</a></button>
        </nav>
      </div>

      <div class="Frame4">
        <div class="upInfoTwo">
          <p class="upInfoTwoPhone">+7 (800) 123 45-67</p>
          <p class="upInfoTwoText">Звонки по России бесплатны</p>
        </div>
      </div>
    </div>


    <div class="Frame73">
      <p class="TextFrame73One">НЕ ЯВЛЯЕТСЯ ПУБЛИЧНОЙ ОФЕРТОЙ. Просим обратить внимание на то, что цены носят информационный и ознакомительный
        характер, а значит ни в какой мере не являются публичной офертой, которая определена в ст. 437 ГК РФ.
        Вся информация на сайте может содержать неточности, орфографические и иные ошибки, она не является полной,
        окончательно и исчерпывающей</p>
      <p class="TextFrame73Two">Разработкой макета занимался Васильев Александр | Что-то на IT’шном
      </p>
    </div>







  </div>
</template>

<style scoped>
.contentFooter {
  background-color: #111827;
  width: 1920px;
  height: 234px;
  color: #F9FAFB;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 24px;
  padding-top: 40px;
}

p {
  color: #F9FAFB;

}

.Frame38 {
  display: flex;
  align-items: center;
  gap: 207px;
}

.Frame2 {
  display: flex;
  flex-direction: column;
  width: 399px;
  height: 98px;
  gap: 8px;
}

img {
  width: 305px;
  height: 74px;
}

.pImg {
  display: flex;
  padding: 0;
  margin: 0;
  gap: 0;
  align-items: center;
}

.smallTextImg {
  font-size: 12px;
  line-height: 16px;
  color: #F9FAFB;
}

.pImg>img {
  width: 16px;
  height: 16px;
  color: #F9FAFB;
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
  background-color: #111827;
  padding: 0;
}

.navBtn>a {
  font-family: 'FormularBold';
  color: #F9FAFB;
}

.navBtn>a:hover {
  color: #8B5CF6;
}

.upInfoTwo {
  width: 351px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 4px;
}

.upInfoTwoPhone {
  font-size: 36px;
  max-height: 40px;
  width: 341px;
  font-family: 'FormularBlack';
}

.upInfoTwoText {
  font-size: 24px;
  width: 351px;
  height: 32px;
  font-family: 'FormularLight';
}

.Frame73 {
  padding-left: 192px;
  padding-right: 192px;

  display: flex;
  gap: 148px;
}

.Frame73>p {
  color: #4B5563;
  font-size: 12px;
  line-height: 16px;
}

.TextFrame73One {
  width: 1146px;
  height: 32px;
}

.TextFrame73Two {
  width: 242px;
  height: 32px;
  text-align: right;
}
</style>