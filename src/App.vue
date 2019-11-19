<template>
    <div id="app">
      <NavBar />
      <!-- <Characters /> -->
      <router-view/>
    </div>
</template>

<script>
import NavBar from '@/components/navbar';

export default {
  name: 'app',
  components: { NavBar },
}
</script>

// <style lang="scss">
// #app {
//   font-family: 'Avenir', Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }
// </style>
