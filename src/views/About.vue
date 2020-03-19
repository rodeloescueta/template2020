<template>
  <v-container fluid pa-0 class="text-center">
    <a @click="goto('/')">Home</a>
    <v-divider
      class="mx-4"
      inset
      vertical
    ></v-divider>
    <span>About</span>
    <br>
    <v-btn @click="alert('about')">alert</v-btn>
    
    
  </v-container>
</template>

<script>
export default {
  name: 'Home',
  data(){
    return{

    }
  },
  methods:{
    goto(val){
      this.$router.push(val)
    }
  }
}
</script>
