<template>
<div>
  <Header />
  <FirstSection />
  <Footer />
  <PopularSection />
  <FashionSection />
  <BestSellingSection />
</div>
</template>

<script>
import Header from './components/Header'
import FirstSection from './components/FirstSection'
import Footer from './components/Footer'
import PopularSection from './components/PopularSection'
import BestSellingSection from './components/BestSellingSection'
import FashionSection from './components/FashsionSection'
export default {
  name: 'App',
  components: {
    Header,
    FirstSection,
    Footer,
    PopularSection,
    BestSellingSection,
    FashionSection
  }
};
</script>


