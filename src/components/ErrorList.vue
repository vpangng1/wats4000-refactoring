<template> 
<div if="errors.length > 0">
      <h2>There was an error fetching weather data.</h2>
      <ul class="errors">
        <li v-for="error in errors">{{ error }}</li>
      </ul>
    </div>
  </div>
</template>


export default {
  name: 'ErrorList',
  data () {
    return {
     
    }
  },
props: {
    weatherData: []
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.errors li {
  color: red;
  border: solid red 1px;
  padding: 5px;
}

</style>