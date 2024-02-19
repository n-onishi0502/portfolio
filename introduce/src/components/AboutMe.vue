<template>
  <v-container>
    <v-row>
      <v-col class="d-flex flex-row justify-center">About Me</v-col>
    </v-row>
    <v-row>
      <v-col class="rounded-pill d-flex flex-row justify-center" >
        <v-avatar size="128">
          <v-img src="../assets/face_smile_man4.png"></v-img>
        </v-avatar>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="d-flex flex-row justify-center">
        <v-card width="90%">
          <v-container>
            <v-row>
              <v-col cols="4" class="d-flex flex-row justify-end">名前：</v-col>
              <v-col cols="6">大西直輝</v-col>
            </v-row>
            <v-row>
              <v-col cols="4" class="d-flex flex-row justify-end">生年月日：</v-col>
              <v-col cols="6">1996/05/02</v-col>
            </v-row>
            <v-row>
              <v-col cols="4" class="d-flex flex-row justify-end">性別：</v-col>
              <v-col cols="6">男</v-col>
            </v-row>
            <v-row>
              <v-col cols="4" class="d-flex flex-row justify-end">経歴：</v-col>
              <v-col cols="6">2019年4月よりIT業界に参入、Java、js/jQuery/vue.js、PHP/laravel/fuelPHP、iOS/android、C#等の様々な言語や環境での案件に対応</v-col>
            </v-row>
          </v-container>
        </v-card>
      </v-col>
    </v-row>  
  </v-container>
</template>

<script>

  export default {
    data: () => ({
    }),
  }
</script>