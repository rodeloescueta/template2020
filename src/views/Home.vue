<template>
  <v-container fluid pa-0 class="text-center">
    <span>Home</span>
    <v-divider
      class="mx-4"
      inset
      vertical
    ></v-divider>
    <a @click="goto('/about')">About</a>
    <br>
    <v-btn @click="alert('home')">alert</v-btn>
    
    
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
