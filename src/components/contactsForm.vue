<script setup>

</script>

<template>
  <div class="content">
    <div class="headerContacts">Остались вопросы?</div>
    <form>
      <div class="two">
        <input class="input" type="text" name="" id="" placeholder="Имя">
        <input class="input" type="text" name="" id="" placeholder="Почта">
      </div>
      <div class="two">
        <input class="input" type="text" name="" id="" placeholder="Телефон">
        <input class="input" type="text" name="" id="" placeholder="Тема вопроса">
      </div>
      <!-- <input class="sms" type="text" placeholder="Сообщение..."> -->
      <textarea class="input sms" name="" id="" placeholder="Сообщение..."></textarea>
    </form>

    <button class="order">Оставить заявку</button>
  </div>
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  justify-content: center;
  overflow: hidden;
  background-color: #fff;
  padding-top: 64px;
  margin-top: 72px;
  border-radius: 16px;
  /* margin-bottom: 72px; */
}

.headerContacts {
  font-family: 'FormularBlack';
  font-size: 30px;
  line-height: 36px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 24px;
  width: 496px;
  padding-top: 12px;
}

.input {
  border: 2px solid #111827;
  width: 493px;
  height: 45px;
  border-radius: 4px;
  padding-left: 12px;
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

.sms {
  max-width: 482px;
  max-height: 135px;
  min-width: 482px;
  min-height: 135px;
  padding: 0;
  padding-left: 12px;
  padding-top: 12px;
}

.order {
  width: 497px;
  height: 44px;
  margin-bottom: 64px;
}

</style>