<template>
  <v-layout class="d-flex align-start flex-column py-6">
    <div class="text-h4 mb-5" block>Bizning afzalliklarimiz</div>

    <div class="cards d-flex flex-wrap">
      <div class="card ma-2 d-flex justify-space-between">
        <img src="../assets/img/afzalliklar-logo-online.svg" alt="">
        <div class="d-flex flex-column pa-3 align-baseline">
          <div class="text-h5">Onlayn akademiya</div>
          <div>
            «Najot Ta'lim» digital academy — bu zamonaviy kasblar o'qitiladigan onlayn akademiya. Qayerda bo'lishingizdan
            qat'i nazar: uydami yo mehmonda, daladami yo safarda — o'zingizga qulay tarzda va vaqtda bilim olishingiz
            mumkin,
            internet va noutbuk bo'lsa bas.
          </div>
        </div>
      </div>

      <div class="card ma-2 d-flex justify-space-between">
        <img src="../assets/img/afzalliklar-logo-star.svg" alt="">
        <div class="d-flex flex-column pa-3 align-baseline">
          <div class="text-h5">O'z ishining ustalari</div>
          <div>
            Darslar katta tajribaga ega malakali mutaxassislar tomonidan tayyorlangan. O'z ishining ustalaridan yanada
            ishonchli bilim va tajribaga ega bo'lasiz
          </div>
        </div>
      </div>

      <div class="card ma-2 d-flex justify-space-between">
        <img src="../assets/img/afzalliklar-logo-pc.svg" alt="">
        <div class="d-flex flex-column pa-3 align-baseline">
          <div class="text-h5">Shunchaki kurs emas</div>
          <div>
            Har bir o'quv kursi shunday ishlab chiqilganki, ularni muvaffaqiyatli yakunlab, siz zamonaviy kasb egasiga
            aylanishingiz va shu sohada o'z faoliyatingizni boshlashingiz mumkin. Hammasi o'z qo'lingizda.
          </div>
        </div>
      </div>

      <div class="card ma-2 d-flex justify-space-between">
        <img src="../assets/img/afzalliklar-logo-target.svg" alt="">
        <div class="d-flex flex-column pa-3 align-baseline">
          <div class="text-h5">Interaktiv darslar</div>
          <div>
            Darslarni o'zlashtirish davrida sizda savollar tug'ilishi tabiiy holat. Mentorlarga murojaat qilishingiz,
            o'zingizni qiziqtirgan savollarizga javob olishingiz va tavsiyalar olishingiz mumkin
          </div>
        </div>
      </div>




      <v-expand-transition>
        <div v-show="show" >
          <div class="cards d-flex flex-wrap">
            <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-practise.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Nazariya va amaliyot</div>
              <div>
                Siz har bir kursda berilgan topshiriqlarni amalga oshirish orqali bilimlaringizni yanada mustahkamlab
                borasiz
              </div>
            </div>
          </div>

          <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-guede.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Mentor kerakmi?</div>
              <div>
                Darslarni o'zlashtirish davrida sizda savollar tug'ilishi tabiiy holat. Mentorlarga murojaat qilsangiz,
                ular
                sizni qiynayotgan masalalar bo'yicha yechim topishga yo'l ko'rsatadilar.
              </div>
            </div>
          </div>

          <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-meeting.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Hamjamiyat</div>
              <div>
                Kursni boshlashingiz bilan “Najot Ta'lim” yopiq hamjamiyatiga a'zo bo'lasiz. Bu yerda siz o'rganishga va
                tajriba almashishga tayyor odamlarni uchratasiz va tanishasiz
              </div>
            </div>
          </div>

          <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-pc2.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Hammamiz insonmiz</div>
              <div>
                O'qish jarayonida avvalgi o'tilgan mavzular yoddan ko'tarilishi, ba'zi mavzularni mustahkamlashga ehtiyoj
                tug'ilishi mumkin. Shu bois sizda avvalgi darslarni takroran ko'rish imkoniyati bor.
              </div>
            </div>
          </div>

          <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-certificate.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Sertifikat</div>
              <div>
                Kursni muvaffaqiyatli yakunlaganingizdan so'ng sizga elektron sertifikat taqdim etiladi. Sertifikat sizni
                bilimingizni oson ko'rsatib beruvchi isbot
              </div>
            </div>
          </div>

          <div class="card ma-2 d-flex justify-space-between">
            <img src="../assets/img/afzalliklar-logo-pay.svg" alt="">
            <div class="d-flex flex-column pa-3 align-baseline">
              <div class="text-h5">Tezkor to'lov</div>
              <div>
                Xaridni eng ommabop to'lov tizimlari orqali bir zumda amalga oshiring va kursni qo'lga kiriting. Hammasi
                onlayn, hammasi zamonaviy, hammasi oson..
              </div>
            </div>
          </div>
          </div>

        </div>
      </v-expand-transition>


      
    </div>
    <v-btn id="card-btn" :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show = !show" color="green-accent-4"></v-btn>
  </v-layout>
</template>


<script>
export default {
  data: () => ({
    show: false,
  }),
}
</script>


<style scoped>
.card {
  width: 45%;
}

.card img {
  width: 60px;
  height: 60px;
}

@media screen and (max-width: 700px) {
  .card {
    width: 90%;
  }
}</style>