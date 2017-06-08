<template>
  <div class="shop-car">
  	<price></price>
  	<num></num>
		<label for="label">总价:</label>
		<span @increment='incrementFun'>{{total}}</span>
  </div>
</template>

<script>
import price from './price';
import num from './num';
export default {
  name: 'shop-car',
  data () {
    return {
      total: 7
    }
  },
  methods:{

  	incrementFun:function(n){
  		console.log(price.price);
  		console.log(num.nowNum);

  		this.total = price.price * n

  	}
  },
  components:{
  	price,
  	num

  }
}
</script>


<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
