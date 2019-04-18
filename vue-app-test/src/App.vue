<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span class="font-weight-light">VUE APP TEST</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="Home"
      >
        <span class="mr-2">Home</span>
      </v-btn>
      <v-btn
        flat
        href="About"
      >
        <span class="mr-2">About</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <FirstComponent/>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from '@/components/HelloWorld'
import FirstComponent from '@/components/FirstComponent'
import Home from '@/views/Home'
import About from '@/views/About'

export default {
  name: 'App',
  home: Home,
  about: About,
  components: {
    HelloWorld,
    FirstComponent,
  },
  data () {
    return {
      //
    }
  }
}
</script>
