<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
      clipped
    >
      <v-list dense>
        <v-list-item v-for="(item,i) in menu" :key="i" :to="item.to">
          <v-list-item-action>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{item.title}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      clipped-left flat
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="hidden-md-and-up"/>
      <v-img 
        contain
        class="mr-5 ml-5"
        height="48"
        width="128"
        max-width="128"
        :src="require('@/assets/logo.png')"/>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn
          v-for="item in menu"
          :key="item.title"
          :to="item.to"
          text
        >{{ item.title }}</v-btn>
      </v-toolbar-items>
      
    </v-app-bar>

    <v-content>
      <router-view/>
    </v-content>

    <v-footer app>
      <span>&copy; rodeloescueta</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      drawer: false,
      menu: [
        {title: 'Home', to: "/", icon: "mdi-home"},
        {title: 'About', to: "about", icon: "mdi-account"},
        {title: 'Contacts', to: "home", icon: "mdi-mail"}
      ]
    }),
    created () {
      // this.$vuetify.theme.dark = true
    },
  }
</script>
