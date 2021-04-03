<template>
  <div class="item absencesWrapper">
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
  name: 'absencesCard',
  props: {
    header: String,
    footer: String
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