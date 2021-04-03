<template>
  <div class="item payRollWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
      </div>
    <div class="body"></div>
     <div class="title footer">
      <p class="footer_letters">
      {{ footer }}
      </p>
      <img class="footer_icon" src="../assets/arrow.png"/>
      </div>
  </div>
</template>

<script>
export default {
  name: 'payRollCard',
  props: {
    header: String,
    footer:String,
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