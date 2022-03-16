<template>
  <v-app>
      <TopBar/>
    <v-main>
     <Home/>
    </v-main>
  </v-app>
</template>

<script>
import TopBar from './components/shared/TopBar'
import Home from './components/Home'
export default {
  name: 'App',

  components: {
   TopBar,
   Home,
  },

  data: () => ({
    //
  }),
};
</script>
