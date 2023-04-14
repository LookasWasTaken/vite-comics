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