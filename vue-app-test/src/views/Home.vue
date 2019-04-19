<template>
  <div class="home">
    <div class="container">
        <!-- <Card msg='Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur debitis voluptate error obcaecati doloribus laborum eius reiciendis, deleniti temporibus iure delectus voluptas, autem quo unde explicabo qui culpa sapiente quae!'></Card> -->
      <Card></Card>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Card from '@/components/Card.vue'


export default {
  name: 'home',
  components: {
    HelloWorld,
    Card,
  }, 
}
</script>
