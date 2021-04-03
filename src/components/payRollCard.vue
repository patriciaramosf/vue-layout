<template>
  <div class="item payRollWrapper">
    payRollCard
  </div>
</template>

<script>
export default {
  name: 'payRollCard',
  props: {
    msg: String
  }
}
</script>
<style>
.payRollWrapper{
  grid-column-start: 10;
  grid-column-end: 13;
  grid-row-start:3;
  grid-row-end:8;
}
</style>