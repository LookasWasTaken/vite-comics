<script>
import SiteHeader from './components/SiteHeader.vue';
import ExternalSites from './components/ExternalSites.vue';
import SiteFooter from './components/SiteFooter.vue';
import CardContainer from './components/CardContainer.vue';
export default {
  data() {
    return {
    }
  },
  components: {
    SiteHeader,
    ExternalSites,
    SiteFooter,
    CardContainer,
  }
}
</script>

<template>

  <SiteHeader></SiteHeader>

  <main>
    <section id="main_section" class="bg-dark">
      <div class="container py-5">
        <CardContainer></CardContainer>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>
  <SiteFooter></SiteFooter>

</template>

<style lang="scss" scoped>
</style>