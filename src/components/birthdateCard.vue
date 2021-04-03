<template>
  <div class="item birthdateWrapper">
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
  name: 'birthdateCard',
  props: {
    header: String,
    footer:String,
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