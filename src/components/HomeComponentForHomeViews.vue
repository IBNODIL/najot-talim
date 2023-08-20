<template>
  <v-container class="pt-16 d-flex justify-space-between">
    <div id="bg" class="mt-12 pb-12">
      <div class="text-h4 font-weight-bold">Kasblarni</div>
      <div class="text-h4 font-weight-bold">
        <div>
          <p class="animaton-text text-1">"Najot Ta'limda" <span>da</span></p>
          <p class="animaton-text text-2">mutaxassislardan</p>
          <p class="animaton-text text-3">onlayn</p>
          <p class="animaton-text text-4">istalgan nuqtadan</p>
        </div>
        <br>
        o'rganing
      </div>

      <p class="mt-6">
        O'zingizga qulay vaqtda, joyda va uslubda
      </p>
      <p class="mb-12">
        zamonaviy kasblarni o'rganing.
      </p>

      <button id="look-to-all-curses">
        Kurslarni ko'rish
      </button>
    </div>

    <div class="empty-place"></div>
  </v-container>
</template>


<script>
export default {
  mounted(){
    document.getElementById('bg').parentElement.classList.add('bg')
  }
}
</script>


<style scoped>
* {
  margin: 0;
  padding: 0;
}

.empty-place{
  max-width: 50%;
}

.bg{
  overflow: visible;
  background-image: url('../assets/img/home-bg-img.svg');
  background-image: url('../assets/img/home-img.png');  
  background-position: right bottom;
  background-repeat: no-repeat;
  background-size: 58%;
  min-height: 75vh;
}

h2 {
  display: block;
}

.animaton-text {
  color: #B5976E;
  opacity: 0;
  transform: translateY(-10px);
  position: absolute;
  animation-duration: 8s;
  animation-timing-function: ease-in;
  animation-iteration-count: infinite;
}

p {
  color: #757575;
}

.animaton-text span {
  color: black;
}

.text-1 {
  animation-name: animation1;
}

.text-2 {
  animation-name: animation2;
}

.text-3 {
  animation-name: animation3;
}

.text-4 {
  animation-name: animation4;
}

#look-to-all-curses{
  padding: 12px 35px;
  background-color: #B5976E;
  border-radius: 50px;
  font-weight: 700;
  border: 2px solid #B5976E;
  transition: all 0.2s ease-in;
  color: white;
}

#look-to-all-curses:hover{
  background-color:white;
  color: black;
}

#look-to-all-curses:active{
  background-color:#B5976E;
  color: white;
}



@media screen and (max-width: 950px) {
  #bg{
    padding-left: 30px;
  }
}

@media screen and (max-width: 590px) {
  .bg{
    background-image: none;
  }
}

@keyframes animation1 {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  5% {
    opacity: 1;
    transform: translateY(0px);
  }

  20% {
    opacity: 1;
    transform: translateY(0px);
  }

  25% {
    opacity: 0;
    transform: translateY(10px);
  }

  100% {
    opacity: 0;
    transform: translateY(-10px);
  }
}

@keyframes animation2 {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  25% {
    opacity: 0;
    transform: translateY(-10px);
  }

  30% {
    opacity: 1;
    transform: translateY(0px);
  }

  45% {
    opacity: 1;
    transform: translateY(0px);
  }

  50% {
    opacity: 0;
    transform: translateY(10px);
  }

  100% {
    opacity: 0;
    transform: translateY(-10px);
  }
}

@keyframes animation3 {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  50% {
    opacity: 0;
    transform: translateY(-10px);
  }

  55% {
    opacity: 1;
    transform: translateY(0px);
  }

  70% {
    opacity: 1;
    transform: translateY(0px);
  }

  75% {
    opacity: 0;
    transform: translateY(10px);
  }

  100% {
    opacity: 0;
    transform: translateY(-10px);
  }
}

@keyframes animation4 {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  75% {
    opacity: 0;
    transform: translateY(-10px);
  }

  80% {
    opacity: 1;
    transform: translateY(0px);
  }

  95% {
    opacity: 1;
    transform: translateY(0px);
  }

  100% {
    opacity: 0;
    transform: translateY(10px);
  }
}
</style>