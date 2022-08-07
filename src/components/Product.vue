<template>
    
    <div class="product">
        <div class="product-inner">
            <div class="product-image-wrap">
                <img :src="product.src" class="image" />
            </div> 
            <div class="product-detail">
                <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi vitae efficitur enim. Integer at sem at elit pulvinar placerat. Proin fermentum eget dolor in efficitur. 
                 Etiam turpis nulla, pharetra a sodales auctor, interdum eu orci.</p>
                <button class="button">READ MORE</button>
            </div>
        </div> 
        
    </div>

</template>

<script>
export default {
    name: 'product',
    props: ['product']
}
</script>


<style>
.product {
    flex: 1 1 33.333%;
    width: 100%;
    padding: 25px;
    margin-bottom:5%;
    
}

.product:hover{
    box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.50);
}

.products {
  display:flex;
  max-width:1288px;
  padding:25px;
  
}

.product-inner{
  position: relative;
  padding: 25px;
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
  border-radius: 8px;
}

.product-image-wrap .image{
  width:90%;
  display: block;  
  margin-left: auto;  
  margin-right: auto; 
}

.product-image-wrap .image:hover{
 width:100%;
 display: block;  
 margin-left: auto;  
 margin-right: auto; 
}

.product-detail {
    text-align:center;
}

#p1,#p2{
   height:25px;
   width:25px;
   border-radius:50% 0 0 50%;
   background-color:blue;  
}

#p2{
   border-radius:0 50% 50% 0;
}
   
.button {
  background-color: white;
  border-style: solid;
  color: black;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  margin:6px 2px;
  cursor: pointer;
  border-radius: 16px;
  font-weight: bold;
}

.button:hover {
  background-color: #f1f1f1;
}


</style>