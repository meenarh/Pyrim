<template>
<div>
  <Header />
  <FirstSection />
  <PopularSection />
  <BestSellingSection />
</div>
</template>

<script>
import Header from './components/Header'
import FirstSection from './components/FirstSection'
import PopularSection from './components/PopularSection'
import BestSellingSection from './components/BestSellingSection'
export default {
  name: 'App',
  components: {
    Header,
    FirstSection,
    PopularSection,
    BestSellingSection
  }
};
</script>


