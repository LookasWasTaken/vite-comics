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