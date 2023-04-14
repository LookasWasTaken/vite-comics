<script>
  export default {
    name: "CardBox",
    props: {
      img: String,
      title: String,
    }
  }
</script>

<template>
<div class="p-1 text-center">
  <img class="img-fluid" :src="img" :alt="title + `Image`">
<h5>{{ title }}</h5>
</div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;

img {
  aspect-ratio: 1/1;
  object-fit: contain;
}

h5{
  color: $light;
  font-size: 0.95rem;
  margin: 1rem 0;
  text-transform: uppercase;
  font-weight: 500;

}
</style>