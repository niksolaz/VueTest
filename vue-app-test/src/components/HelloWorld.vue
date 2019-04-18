<template>
  <v-container>
    <v-layout justify-center>
      <h2 class="headline font-weight-bold mb-3">
      <a
        :href="ecosystem.href"
        class="subheading mx-3"
        target="_blank"
      >
        {{ ecosystem.text }}
      </a>
      </h2>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      ecosystem: {
          text: 'My Github',
          href: 'https://github.com/niksolaz/VueTest'
        },
    })
  }
</script>

<style>

</style>