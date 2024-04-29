<template>
  <div class="hello">
    <h1>Acoustic panels</h1>
  
<p>width of the room  </p>
<input v-model="RoomWidth">
<h2>{{RoomWidth}}</h2> <p>inches </p>
<p>__________________________________________</p>
<p>length of the room </p>
<h2> {{RoomLength}}</h2><p>inches </p>
<input v-model="RoomLength">
<br>
<br>
<button @click="panelsCalc(RoomWidth, RoomLength)">Calculate</button>
<h2>{{panels}} panels needed</h2>
  <p>asuming the size of one panel is 288 square inches</p>
    </div>
</template>

<script>
export default {
  components: {},
 data() {
        return {RoomWidth: 0, RoomLength: 0, panels:0}
    },
    async created () {
     

  },
  
  methods: {

    async panelsCalc( RoomWidth, RoomLength){
      this.panels = ((RoomWidth * RoomLength))/288
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
