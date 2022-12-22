<template>
<div>
  <Header />
  <FirstSection />
  <Footer />
</div>
</template>

<script>
import Header from './components/Header'
import FirstSection from './components/FirstSection'
import Footer from './components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    FirstSection,
    Footer
  }
};
</script>


