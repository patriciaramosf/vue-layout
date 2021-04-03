<template>
  <div class="item exitWrapper">
    exitsCard
  </div>
</template>

<script>
export default {
  name: 'exitsCard',
  props: {
    msg: String
  }
}
</script>
<style>
.exitWrapper{
  grid-column-start: 10;
  grid-column-end: 13;
  grid-row-start:1;
  grid-row-end:3;
}
</style>