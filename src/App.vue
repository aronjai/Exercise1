<template>
<div class="head">
 <p class="text">Hello Developer!</p>
 <p class="smalltext">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
</div> 
  <main id="app">
    <section class="products"></section>
    <ProductCard
      v-for="product in products"
      :product="product"
    />

  </main>
</template>

<script>
import ProductCard from './components/Product';
export default {
  name: 'App',
  components: {
    ProductCard
  },
  data() {
    return{
     products:[
       {
       title: "card1",
       src: require('./assets/smallcards.png')
       },
       {
       title: "card2",
       src: require('./assets/smallcards.png')
       },
       {
       title: "card3",
       src: require('./assets/smallcards.png')
       },
     ] 
    }
  }
}
</script>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  
}



 

@media screen and (min-width: 600px) {

  body{
  background-image: url("./assets/header1.png");
  font-family: 'monseratt', sans-serif;
  background-repeat: no-repeat;
  background-size: 100% auto;
  font-size:1vw;
  

  }
  
  main {
  width: 100vw;
  min-height: 1vh;
  overflow:hidden;


  display:flex;
  justify-content: center;
  align-items:center; 
  }

  .text{
  color:#fff;
  font-size:5vw;
  font-family: arial;
  text-align: center;
  padding-top: 1.5em;
  
  }

  .text:hover{
    color:black;
    cursor: pointer;
  }

  .smalltext{
  color:#fff;
  font-size:2vw;
  font-family: arial;
  text-align: center;
  padding-top: 1.5em;

  }

  .head {
  background: rgba(0,0,0,0.4);
  height: auto;
  padding-top: 6%;
  padding-bottom:9%;
  }
  
  
}


@media screen and (max-width:600px) {
  body{
  
  background-image: url("./assets/header2.png");
  font-family: 'monseratt', sans-serif;
  background-repeat: no-repeat;
  background-size: 100% auto;
  font-size:1em;


  }

  main {

  min-height: 100vh;
  overflow:hidden;
  width: 100%;
  display: block;
  margin-bottom: 20px;

  }

   .text{
  color:#fff;
  font-size:15vw;
  font-family: arial;
  text-align: center;
  padding-top: 1.5em;
  font-weight: 550;
  
 .text:hover{
    color:black;
    cursor: pointer;
  }

  }

  .smalltext{
  color:#fff;
  font-size:8vw;
  font-family: arial;
  text-align: center;
  padding-top: 1.5em;
  padding-right:5px;
   padding-left: 20px;


  }

  .head {
  background: rgba(0,0,0,0.4);
  height: auto;
  padding-bottom:6%;
  }
  
  
}



</style>
