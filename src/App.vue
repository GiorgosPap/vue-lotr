<template>
    <div id="app">
      <NavBar />
      <Characters />
    </div>
</template>

<script>
import NavBar from '@/components/navbar';
import Characters from '@/components/characters';

export default {
  name: 'app',
  components: { NavBar, Characters },
}
</script>
