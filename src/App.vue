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
    <div class="jumbo">
      <img class="w-100" src="./assets/img/jumbotron.jpg" alt="Jumbotron">
    </div>
    <section id="main_section" class="bg-dark">
      <div class="container py-3 text-center">
        <h4 class="current_series">CURRENT SERIES</h4>
        <CardContainer></CardContainer>
        <button class="load">LOAD MORE</button>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>
  <SiteFooter></SiteFooter>

</template>

<style lang="scss" scoped>
@use "./assets/scss/partials/variables" as *;
.jumbo{
  height: 430px;
  overflow: hidden;
}

.current_series{
  color: $light;
  background-color: $accent;
  width: max-content;
  padding: 0.5rem 1rem;
  transform: translate(0, -80%);
}

.load{
  font-weight: 500;
  color: $light;
  background-color: $accent;
  width: max-content;
  padding: 0.5rem 5rem;
  border: none;
  margin: 2rem 0.5rem;
}
</style>