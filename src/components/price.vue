<template>
  <div class="price">
  	<button>{{price}}</button>
  </div>
</template>

<script>
export default {
  name: 'price',
  data () {
    return {
      price: 3.79
    }
  },
  methods:{

  }
}
</script>


<style scoped>
.price{
	margin-bottom: 10px;
}
</style>
