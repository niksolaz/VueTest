<template>
  <div class="card" style="width: 18rem;">
    <img src="https://fakeimg.pl/250x100/66ff66/?text=Card&font=lobster" class="card-img-top" alt="">
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ msg }}</p>
      <a href="#" class="btn btn-primary" @click='changeText()'>Go somewhere</a>
    </div>
  </div>
</template>



<script>
export default {
  name: 'Card',
  data (){
    return {
      title : 'my Title',
      elem: true,
      msg: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur debitis voluptate error obcaecati doloribus laborum eius reiciendis, deleniti temporibus iure delectus voluptas, autem quo unde explicabo qui culpa sapiente quae!',
    }
  },
  // props: {
  //   msg: String
  // },
  methods: {
    changeText(){
      this.elem = !this.elem;
      console.log(this.elem);
      if( this.elem == true ) { 
        this.title = "Title TRUE";
        this.msg = 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur debitis voluptate error obcaecati doloribus laborum eius reiciendis, deleniti temporibus iure delectus voluptas, autem quo unde explicabo qui culpa sapiente quae!';
      }
      if( this.elem == false ) {
        this.title = "Title FALSE";
        this.msg = '';
      }
    }
  }
}
</script>
