<template>
  <div class="item holidaysWrapper">
    holidaysCard
  </div>
</template>

<script>
export default {
  name: 'holidaysCard',
  props: {
    msg: String
  }
}
</script>
<style>
.holidaysWrapper{
  grid-column-start: 1;
  grid-column-end: 5;
  grid-row-start:5;
  grid-row-end:9;
}
</style>