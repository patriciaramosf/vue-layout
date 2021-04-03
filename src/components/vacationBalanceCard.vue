<template>
  <div class="item vacationWrapper">
    vacationBalanceCard
  </div>
</template>

<script>
export default {
  name: 'vacationBalanceCard',
  props: {
    msg: String
  }
}
</script>
<style>
.vacationWrapper{
  grid-column-start: 5;
  grid-column-end: 8;
  grid-row-start:5;
  grid-row-end:8;
}
</style>