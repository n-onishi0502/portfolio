<template>
  <v-app-bar app elevate-on-scroll 
    src="https://fastly.picsum.photos/id/46/3264/2448.jpg?hmac=ZHE8nk-Q9uRp4MxgKNvN7V7pYFvA-9BCv99ltY3HBv4"
  >
    <v-tabs>
      <v-tab to="/">
        <v-icon>
          mdi-home
        </v-icon>
      </v-tab>
      <v-tab class="hidden-sm-and-down" 
        @click="$vuetify.goTo('#aboutMe')"
        v-bind="aboutMe"
      >About Me</v-tab>
      <v-tab class="hidden-sm-and-down"
        @click="$vuetify.goTo('#skills')"
        v-bind="skills"
      >Skills</v-tab>
      <v-tab class="hidden-sm-and-down" to="/career">Career</v-tab>
    </v-tabs>
    <v-app-bar-nav-icon right class="hidden-md-and-up ml-auto" @click="drawer=true"></v-app-bar-nav-icon>
    <v-navigation-drawer app v-model="drawer" right fixed temporary>Navigation Lists</v-navigation-drawer>
  </v-app-bar>
</template>

<script>


// import Welcome from '../components/Welcome'

  export default {
    data: () => ({
      drawer: null,
    }),
  }
</script>