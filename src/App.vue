<template>
<div>
  <Header />
  <FirstSection />
  <PopularSection />
  <FashionSection />
  <BestSellingSection />
  <Footer />

</div>
</template>

<script>
import Header from './components/Header'
import FirstSection from './components/FirstSection'
import PopularSection from './components/PopularSection'
import BestSellingSection from './components/BestSellingSection'
import Footer from './components/Footer'
import FashionSection from './components/FashsionSection'
export default {
  name: 'App',
  components: {
    Header,
    FirstSection,
    PopularSection,
    BestSellingSection,
    FashionSection,
    Footer
  }
};
</script>
