<template>
  <div id="app">
    <!-- HEADER -->
    <Header />
    <!-- MAIN -->
    <!-- FOOTER -->
  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
// GENERAL
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  font-family: 'Fira Sans Condensed', sans-serif;
  font-size: 14px;
}
// UTILITIES
  .container{
    max-width: 1200px;
    margin: 0 auto;
  }
  // Flex
  .flex{
    display: flex;
  }
  .jc-between{
    justify-content: space-between;
  }
  .ai-center{
    align-items: center;
  }
</style>
