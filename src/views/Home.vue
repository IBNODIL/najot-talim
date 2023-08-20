<template>
  <div>
    <v-container id="home-grey-bg" class="bg-grey-lighten-3 pa-0">
      <HomeComponent></HomeComponent>
    </v-container>
  </div>

  <v-container id="our-advantage">
    <OurAdvantage></OurAdvantage>
  </v-container>

  <div>
    <v-container id="courses-grey-bg" class="bg-grey-lighten-3 pa-0">
      <Courses></Courses>
    </v-container>
  </div>

  <v-container id="our-advantage">
    <Enders></Enders>
  </v-container>
</template>


<script>
import HomeComponent from '../components/HomeComponentForHomeViews.vue'
import OurAdvantage from '../components/OurAdvantage.vue'
import Courses from '../components/Courses.vue'
import Enders from '../components/Enders.vue'
export default {
  components: {
    HomeComponent,
    OurAdvantage,
    Courses,
    Enders,
  },

  mounted() {
    document.getElementById('home-grey-bg').parentElement.classList.add('bg-grey-lighten-3')
    document.getElementById('courses-grey-bg').parentElement.classList.add('bg-grey-lighten-3')
  }
}
</script>


<style scoped>

</style>