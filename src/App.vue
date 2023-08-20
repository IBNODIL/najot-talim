<template>
  <v-card>
    <v-layout>

      <v-app-bar prominent color="grey-lighten-3" class="elevation-0 py-4">
        <v-container class="pt-2 d-flex">
          <v-toolbar-title>
            <div class="nav-icon"><a href="#"><img src="./assets/img/navbar-logo.svg" alt=""></a></div>
          </v-toolbar-title>

          <v-list bg-color="grey-lighten-3">
            <v-list-item>
              <v-btn :ripple="false" variant="plain" to='/' class="hidden-sm-and-down">Kurslar</v-btn>
              <v-btn :ripple="false" variant="plain" to='/' class="hidden-sm-and-down">Blog</v-btn>
              <button id="login" color="black" to='/'>Kirish</button>
            </v-list-item>
          </v-list>

          <v-app-bar-nav-icon class="hidden-md-and-up" variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

        </v-container>
      </v-app-bar>

      <v-navigation-drawer v-model="drawer" location="left" temporary class="hidden-md-and-up">
        <v-list>
          <v-btn block :ripple="false" variant="plain" to='/'>Kurslar</v-btn>
          <v-btn block :ripple="false" variant="plain" to='/'>Blog</v-btn>
        </v-list>
      </v-navigation-drawer>

      <v-main>
        <RouterView></RouterView>
      </v-main>
    </v-layout>
  </v-card>
</template>


<script>
import { RouterView } from 'vue-router';

export default {
  data: () => ({
    drawer: false,
    group: null,
  }),

  watch: {
    group() {
      this.drawer = false
    },
  },
}
</script>


<style scoped>
  .nav-icon{
    width: 250px;
  }

  #login{
    background-color: white;
    padding: 8px 35px;
    border: 2px solid #fff;
    transition: all 0.2s ease-in;
    border-radius: 50px;
  }

  #login:hover{
    box-sizing: border-box;
    border: 2px solid #B5976E;
  }

  #login:active{
    border: 2px solid #B5976E;
    background-color: #B5976E;
  }

  @media screen and (max-width: 760px) {
    .nav-icon{
      width: 140px;
      margin-top: 15px;
    }
  }
</style>