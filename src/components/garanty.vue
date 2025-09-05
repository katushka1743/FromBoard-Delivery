<script setup>

</script>

<template>
  <div class="content">
    <div class="text">
      <div class="headerGaranty">Гарантии качества</div>
      <p class="textHeaderGaranty">Наши гарантии качества включают в себя полный спектр документов, необходимых
        для ввоза и вывоза товаров,
        а также
        для успешного бизнеса на мировом рынке.
        Мы предоставляем вам надёжность и уверенность</p>
    </div>
    <div class="garantyPoints">
      <div class="garantyPoint">
        <img src="/src/img/Rectangle 3.png" alt="">
        <p class="imgText">Свидетельство о регистрации в РФ</p>
      </div>
      <div class="garantyPoint">
        <img src="/src/img/Rectangle 3-1.png" alt="">
        <p class="imgText">Свидетельство о регистрации в США</p>
      </div>
      <div class="garantyPoint">
        <img src="/src/img/Rectangle 3-2.png" alt="">
        <p class="imgText">Свидетельство о регистрации в Китае</p>
      </div>
      <div class="garantyPoint">
        <img src="/src/img/Rectangle 3-3.png" alt="">
        <p class="imgText">Свидетельство о регистрации в Великобритнии</p>
      </div>
    </div>
    <button class="btnGaranty">Показать больше документов</button>
  </div>
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  gap: 24px;
  align-items: center;

}

.text {
  display: flex;
  flex-direction: column;
  gap: 12px;
  align-items: center;

}

.headerGaranty {
  font-family: 'FormularBlack';
  font-size: 30px;
  line-height: 36px;
}

.textHeaderGaranty {
  font-size: 16px;
  line-height: 24px;
  width: 756px;
  text-align: center;
}

img {
  height: 375px;
}

.garantyPoints {
  display: flex;
  justify-content: space-between;
  gap: 24px;
  padding-bottom: 12px;
}

.garantyPoint {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 366px;
  gap: 4px;
}

.imgText {
  font-size: 18px;
  font-family: 'FormularBold';
  font-family: 'FormularBlack';
  line-height: 28px;
  text-align: center;
}

.btnGaranty {
  width: 315px;
  height: 56px;
  font-size: 16px;
  border-radius: 12px;
}
</style>