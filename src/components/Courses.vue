<template>
  <v-layout class="d-flex align-start flex-column py-6">
    <div class="text-h4 mb-5" block>Yo'nalishlar bo'yicha kurslar</div>
    <div>Zamonaviy sohalardan birini o'rganing va talabgir kasb egasi bo'ling!</div>

    <div class="cards my-5 d-flex flex-wrap">
      <v-card class='card ma-4 pa-5' v-for="card in cards">
        <v-card-title>{{ card.title }}</v-card-title>
        <v-card-subtitle>{{ card.subtitle }}</v-card-subtitle>
      </v-card>
    </div>

    <v-btn color="green" variant="outlained">Barcha kurslarni ko'rish</v-btn>
  </v-layout>
</template>


<script>
export default {
  data (){
    return{
      cards: [
        {
          title: 'SMM onlayn',
          subtitle: `Ijtimoiy tarmoqlar orqali turli biznes va loyihalarni rivojlantirishni o'rganasiz.`,
        },

        {
          title: 'Social Media Design',
          subtitle: `Ijtimoiy tarmoqlar orqali turli biznes va loyihalarni rivojlantirishni o'rganasiz.`,
        },

        {
          title: 'Dasturlash foundation',
          subtitle: `Foundation dasturlash kursida C va Python dasturlash tillari va ular orqali dasturlashning mantiq-mohiyati o’rgatiladi. Kurs davomida dasturlashning fundamental tushunchalari, dasturchining ishini yengillashtirib beradigan texnologiyalar, interfeys va ma’lumotlar bazasi bilan ishlash jarayonlari haqida ma’lumotlar beriladi.`,
        },

        {
          title: 'Adobe Illustrator',
          subtitle: `Adobe Illustrator - vektorli grafikalar (chizmalar) bilan ishlash uchun mo'ljallangan dastur hisoblanadi.`,
        },

        {
          title: '.NET mutaxassislik kursi',
          subtitle: `.NET mutaxassislik kursi yordamida universal C# dasturlash tilida ishlovchi va oʻz faoliyatida .NET platformasi va texnologiyalaridan foydalanuvchi dasturchiga aylaning. C# dasturlash tilining imkoniyatlari va qoʻllash doirasi nihoyatda keng, uni mukammal bilgan dasturchi esa veb-saytlardan tortib mobil va desktop ilovalargacha, oʻyinlardan tortib kross-platformali dasturlargacha qurish imkoniyatiga ega boʻladi.`,
        },

        {
          title: 'Node JS Telegram bot',
          subtitle: `Telegram bot yasash va dasturlashni 0 dan o'rganing!`,
        },

        {
          title: 'Kompyuter savodxonligi kursi',
          subtitle: `Ushbu kurs orqali kompyuterdan foydalanish bo'yicha asosiy bilimlarni olishingiz mumkin.`,
        },

        {
          title: 'HBS AKADEMIYASI',
          subtitle: `Noldan professional darajada treyding va investitsiyalarni halol yo'lida savdo qilishni o'rgatuvchi akademiya.`,
        },
      ],
    }
  }
}
</script>


<style scoped>
.card {
  border: 1px solid black;
  border-radius: 5px;
  width: 250px;
}

.card:hover {
  background-color: #fff;
  border: 1px solid #fff;
  transform: scale(1.1);
}</style>