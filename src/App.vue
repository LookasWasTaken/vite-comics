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
      <div class="container">
        <CardContainer></CardContainer>
        <h1 class="m-0 py-5 text-light">Content goes BRRRRRRRR</h1>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>

  <SiteFooter></SiteFooter>

</template>