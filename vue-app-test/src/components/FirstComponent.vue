<template>
<v-container>
  <v-layout justify-center>
    <div>
      <v-flex xs12>
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="50"
        ></v-img>
      </v-flex>
      <v-flex xs12>
        <div
        text-xs-center
        wrap
        class="mb-5"
        >
          <h2>{{ myVar }}</h2>
        </div>
      </v-flex>

      <v-flex xs12>
        <v-btn @click="myVar = 'Hi, I am John Doe'">Name</v-btn>
        <v-btn @click="myVar = 'this is my phone: +47 1234567890 '">Cell</v-btn>
        <v-btn @click="myVar = 'this is my email: johndoe@info.com'">Email</v-btn>
      </v-flex>
    </div>
  </v-layout>
</v-container>
</template>

<script>
  export default {
    name: 'FirstComponent',
    data(){
      return {
        myVar:'',
      }
    },
  }
</script>


<style>
  
</style>
