<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <Main />

    <!-- FOOTER -->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
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
  color: #fff;
}
a{
  text-decoration: none;
}
img{
  max-width: 100%;
}

// UTILITIES
  .container{
    max-width: 1270px;
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
