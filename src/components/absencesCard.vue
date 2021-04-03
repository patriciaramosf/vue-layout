<template>
  <div class="item absencesWrapper">
    absencesCard
  </div>
</template>

<script>
export default {
  name: 'absencesCard',
  props: {
    msg: String
  }
}
</script>
<style>
.absencesWrapper{
  grid-column-start: 1;
  grid-column-end: 5;
  grid-row-start:1;
  grid-row-end:5;
}
</style>