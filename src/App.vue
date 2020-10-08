<template>
  <main class="font-sans antialiased">
   <Header />
   <Content />
   <Footer />
  </main>
</template>

<script>
import Header from "./components/Header"
import Content from "./components/Content"
import Footer from "./components/Footer"
  export default {
    components:{
      Header,
      Content,
      Footer,
    }
  }
</script>
