<script setup>
import { ref, computed } from "vue";

const reviews = ref([
  {
    text: "Я заказала последний iPhone из США через ваш сервис, и доставка прошла быстро и без каких-либо проблем. Гарантии качества и надёжная упаковка сделали мой опыт покупки невероятно позитивным",
    name: "Анна",
  },
  {
    text: "Я уже несколько лет заказываю дизайнерскую одежду из Франции через ваш сервис, и он никогда меня не подводил. Важно иметь надёжную компанию, которая позаботится о вашем заказе и предоставит все необходимые документы для ввоза в Россию",
    name: "Алексей",
  },
  {
    text: "Я заказал редкий антикварный предмет из Японии через ваш сервис, и остался впечатлен. Все пришло в отличном состоянии, и ваша гарантия качества действительно работает. Спасибо за ваше профессиональное обслуживание",
    name: "Дмитрий",
  },
  {
    text: "Заказал шикарные часы из Швейцарии, и доставка была невероятно быстрой. Ваш сервис делает интернет-шоппинг более доступным и удобным",
    name: "Игорь",
  },
  {
    text: "Ваш сервис действительно изменил мой способ покупок. Я больше не переживаю о таможенных вопросах и документах - все у вас в порядке. Спасибо за ваше качество и надежность",
    name: "Екатерина",
  },
]);

// // Индекс первого видимого отзыва
// const currentIndex = ref(0);

// // Сколько карточек видно за раз (у тебя в вёрстке сейчас по 2)
// const visibleCount = 2;

// // При нажатии "вперёд"
// function Plus() {
//   currentIndex.value = (currentIndex.value + 1) % reviews.value.length;
// }

// // При нажатии "назад"
// function Minus() {
//   currentIndex.value =
//     (currentIndex.value - 1 + reviews.value.length) % reviews.value.length;
// }

// // Стили для сдвига всей ленты
// const trackStyle = computed(() => ({
//   transform: `translateX(-${(100 / visibleCount) * currentIndex.value}%)`, // сдвигаем по индексу
//   transition: "transform 0.5s ease", // плавная анимация
//   width: `${(reviews.value.length / visibleCount) * 100}%`, // ширина всей ленты
// }));

const currentIndex = ref(0)
const visibleCount = 2
const cardWidth = 626
const gap = 24

// ширина всей ленты
const trackStyle = computed(() => ({
  transform: `translateX(-${currentIndex.value * (cardWidth + gap)}px)`,
  transition: "transform 0.5s ease",
  width: `${reviews.value.length * (cardWidth + gap)}px`,
  display: "flex",
  gap: `${gap}px`
}))

// кнопка "вперёд"
function Plus() {
  if (currentIndex.value < reviews.value.length - visibleCount) {
    currentIndex.value++
  } else {
    // если дошли до конца — возвращаемся в начало
    currentIndex.value = 0
  }
}

// кнопка "назад"
function Minus() {
  if (currentIndex.value > 0) {
    currentIndex.value--
  } else {
    // если ушли влево за 0 — прыгаем в конец
    currentIndex.value = reviews.value.length - visibleCount
  }
}

</script>


<template>
  <div class="content">

    <div class="headerReviews">Отзывы</div>
    <div class="vectorsMain">
      <div class="vector">
        <button @click="Minus">
          <img src="/src/img/Vector (1).png" alt="">
        </button>
      </div>

      <div class="slider-window">
        <div class="main" :style="trackStyle">
          <div  class="rectangle" v-for="(review, index) in reviews" :key="index">
            <p class="reviewText">{{ review.text }}</p>
            <p class="reviewName">{{ review.name }}</p>
            <img src="/src/img/Quotes.png" alt="" class="Quotes">
          </div>
        </div>
      </div>

      <div class="vector">
        <button @click="Plus">
          <img src="/src/img/Vector (2).png" alt="">
        </button>
      </div>

    </div>

  </div>

</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 24px;
  justify-content: center;
  overflow: hidden;
}

.headerReviews {
  font-family: 'FormularBlack';
  font-size: 30px;
  line-height: 36px;
}

.vectorsMain {
  display: flex;
  width: 100%; 
  justify-content: space-between;
  align-items: center;
  gap: 47px;
}

button {
  background-color: #E5E7EB;
  padding: 0;
  margin: 0;
}

.slider-window {
  overflow: hidden;
  width: calc(626px * 2 + 24px);
}

.main {
  display: flex;
  gap: 24px;
}

.rectangle {
  background-color: #fff;
  width: 626px;
  height: 350px;
  border-radius: 16px;
  position: relative;

  flex-shrink: 0;
}


.reviewText {
  font-size: 24px;
  font-family: 'FormularBold';
  line-height: 32px;
  width: 540px;
  height: 224px;
  padding: 32px 43px 30px 43px;

}

.reviewName {
  font-family: 'FormularLight';
  font-size: 24px;
  line-height: 32px;
  width: 540px;
  padding-inline: 43px;
  color: #6B7280;
}

.Quotes {
  width: 75px;
  position: absolute;
  right: 18px;
  bottom: 40px;

}
</style>