<template>
  <div class="num">
		<button @click="min">-</button>
		<button>{{nowNum}}</button>
		<button @click="plus">+</button>
  </div>
</template>

<script>

export default {
  name: 'num',
  data () {
    return {
    	minNum:0,
      nowNum: 0,
      plusNum:0
    }
  },
  methods:{
  	plus:function(){
			this.nowNum += 1;
			this.$emit('increment',this.nowNum);
  	},
  	min:function(){
  		if(this.nowNum==0){
  			return
  		}
  		this.nowNum -= 1;
  		this.$emit('increment',this.nowNum)
  	}
  }
}
</script>


<style scoped>
	button{
		padding:0 10px;
	}
.num{
	margin-bottom: 10px;
}
</style>
