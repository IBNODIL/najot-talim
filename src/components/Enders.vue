<template>
  <v-layout class="d-flex align-start flex-column py-6">
    <div class="text-h4 mb-5" block>Bitiruvchilarimizning ish joylari:</div>
    <div>Eng yaxshi bitiruvchilarimiz nufuzli tashkilot va kompaniyalarda faoliyat yuritadi. Zamonaviy kasb egalariga doim
      va har yerda talab yuqori bo‘ladi.</div>

    <div class="cards pl-5 my-5 d-flex flex-wrap">
      <img src="../assets/img/work-place-epam.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-techart.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-humo.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-agrobank.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-davr-bank.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-texnomart.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-soliq.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-uzcard.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-mytaxi.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-faktor.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-jatfon.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-fido-studio.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-osmondagi-bolalar.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-islom-uz.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-cambridge.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-kun-uz.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-yoshlar-agentligi.svg" class='card ma-4 pa-5 job-images'>
      <img src="../assets/img/work-place-pcg.svg" class='card ma-4 pa-5 job-images'>
    </div>
  </v-layout>

<v-layout class="d-flex align-start flex-column py-6">
  <div class="text-h4 mb-5" block>Bitiruvchilarimizdan izohlar</div>
    <div>Oʻquv kurslarimiz, ustozlar, qoʻlga kiritilgan bilim va koʻnikmalar, olingan natijalar haqida bitiruvchilarimizdan eshiting hamda ulardan kerakli tavsiyalar oling.</div>

  <div class="pl-5 my-5 d-flex flex-wrap">
    <VideoComponent
    :video-source="1"
    :title="'20.12.2023'"
    :title2="'Frontend dasturchi'"
    :subtitles="'Salohiddin Dilmatov'"
  ></VideoComponent>

  <VideoComponent
    :video-source="2"
    :title="'20.12.2023'"
    :title2="'SMM-menejer'"
    :subtitles="'Abdumannof Tursunov'"
  ></VideoComponent>

  <VideoComponent
    :video-source="3"
    :title="'20.12.2023'"
    :title2="'Grafik dizayner'"
    :subtitles="'Shahzoda Sunnatillayeva'"
  ></VideoComponent>

  <VideoComponent
    :video-source="4"
    :title="'20.12.2023'"
    :title2="'Art-direktor'"
    :subtitles="'Sayfulloh Asadullayev'"
  ></VideoComponent>
  </div>
</v-layout>

  <v-layout class="d-flex " rounded="">
    <img class="operator" src="../assets/img/operator.jpg" alt="">
    <div color="#F9F8F7" class="operator d-flex align-center justify-center">
      <v-card width="500px" height="500px" class="d-flex flex-column pa-5 justify-space-evenly">
        <v-card-title>Yordam kerakmi?</v-card-title>
        <v-card-subtitle>FAQ boʻlimi ham sizga yordam bera olmadimi? Telefon raqamingizni yozib qoldiring, biz sizga qoʻngʻiroq qilamiz va birorta ham savolingiz javobsiz qolmasligiga harakat qilamiz.</v-card-subtitle>

        <div>
          <v-card-subtitle>
            Ismingizni kiriting
          </v-card-subtitle>
          <v-text-field label="Ali" variant="solo"></v-text-field>
        </div>

        <div>
          <v-card-subtitle>
            Telefon raqamingizni kiriting
          </v-card-subtitle>
          <v-text-field label="+998 99 999 99 99" variant="solo"></v-text-field>
        </div>

        <v-card-subtitle>
          "So‘rov yuborish" tugmasini bosish orqali
Platformadan foydalanish qoidalari ga rozilik bildirasiz.
        </v-card-subtitle>

        <button id="send">
        So'rovnoma yuborish
      </button>
      </v-card>
    </div>
  </v-layout>
</template>


<script>
import VideoComponent from '../components/VideoComponent.vue'
export default {
  data() {
    return {
    };
  },
  components:{
    VideoComponent,
  },
  methods: {
    
  },
};
</script>


<style scoped>
.job-images {
  filter: grayscale(1);
  background-color: rgba(173, 173, 173, 0.526);
  border-radius: 10px;
}

.job-images:hover {
  background-color: white;
  transform: scale(1.1);
  filter: grayscale(0);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.267);
}

.operator{
  width: 50%;
}

#send{
  padding: 12px 35px;
  background-color: #B5976E;
  border-radius: 50px;
  font-weight: 700;
  border: 2px solid #B5976E;
  transition: all 0.2s ease-in;
  color: white;
}

#send:hover{
  background-color:white;
  color: black;
}

#send:active{
  background-color:#B5976E;
  color: white;
}
</style>