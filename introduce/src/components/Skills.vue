<template>
  <v-container class="bgg">
    <v-row>
      <v-col class="d-flex flex-row justify-center">Skills</v-col>
    </v-row>
    <v-row>
      <v-container>言語・フレームワーク</v-container>
    </v-row>
    <v-row max-width="100">
      <v-col
        v-for="[language, progress] in languages"
        :key="language"
        cols="4"
      >
        <v-card height="50">
          <v-container>
            {{ language }}
            <v-progress-linear :value="progress"></v-progress-linear>
          </v-container>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-container>その他</v-container>
    </v-row>
    <v-row>
      <v-col
        v-for="[etc, etcProgress] in etcs"
        :key="etc"
        cols="4"
      >
        <v-card height="50">
          <v-container>
            {{ etc }}
            <v-progress-linear :value="etcProgress"></v-progress-linear>
          </v-container>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

  export default {
    data: () => ({
      languages :[ 
        ['JavaScript',70], ['Vue.js', 70], ['jQuery', 70],['PHP', 50],['FuelPHP', 40],['Laravel', 40], ['HTMLCSS', 60], ['MySQL', 40],['Java', 30], ['C#', 10],['ASP.NET', 10]
      ],
      etcs : [
        ['Git',70], ['npm',50], ['docker',50], ['jenkins', 40], ['backlog',50], ['access',10]
      ],
    }),
  }
</script>

<style>

.bgg{
  background-image:"https://fastly.picsum.photos/id/52/1280/853.jpg?hmac=FBJ023QL6SsJpbQl8B20ExSey3BjyRH1MOw7Uo7fIMU"
}
</style>