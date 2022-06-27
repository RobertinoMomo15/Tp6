<template>

  <section class="src-components-header">

    <div id="header" :style=" win ? {background : pickedColor} : '' ">

      <h1>The Great <br>
        <span id="colorDisplay">
          {{this.$store.state.pickedColor != ''? this.$store.state.pickedColor : 'RGB' }}
        </span>        
        <br>
        Guessing Game</h1>

    </div>

    <NavBar />
  
  </section>

</template>

<script>
  import NavBar from './NavBar.vue'

  export default  {
    name: 'src-components-header',
    props: [],
    components: {
      NavBar
    },
    mounted () {

    },
    data () {
      return {
      }
    },
    methods: {

    },
    computed: {

    }
}

</script>

<style scoped lang="css">
  

  #header {
	transition: all 0.3s;
	background: steelblue;
	text-transform: uppercase;
	text-align: center;
	margin: 0;
	color: white;
  }

  #colorDisplay {
    font-size: 200%;
  }



</style>
