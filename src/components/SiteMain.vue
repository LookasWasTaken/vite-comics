<script>
import CardContainer from './CardContainer.vue';
import ExternalSites from './ExternalSites.vue';
  export default {
    name: "SiteMain",
    data (){
        return {
        }
    },
    components: {
        CardContainer,
        ExternalSites,
    }
  }
</script>

<template>
  <main>
    <div class="jumbo">
      <img class="w-100" src="../assets/img/jumbotron.jpg" alt="Jumbotron">
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
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
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