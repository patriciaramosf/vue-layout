<template>
  <div class="item birthdateWrapper">
    birthdateCard
  </div>
</template>

<script>
export default {
  name: 'birthdateCard',
  props: {
    msg: String
  }
}
</script>
<style>
.birthdateWrapper{
  grid-column-start: 5;
  grid-column-end: 10;
  grid-row-start:1;
  grid-row-end:5;
}
</style>