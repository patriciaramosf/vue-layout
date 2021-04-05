<template>
  <div class="item birthdateWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
      </div>
    <div class="body bodyBirthdate">
      <childBirthdateCard birthdateDescription="Mónica López cumple años el 2 de marzo"/>
      <childBirthdateCard birthdateDescription="Paula Pamela cumple años el 2 de mayo"/>
      <childBirthdateCard birthdateDescription="Jon Doe cumple años el 20 de agosto"/>
      <childBirthdateCard birthdateDescription="Mónica López cumple años el 2 de marzo"/>
      <childBirthdateCard birthdateDescription="Mónica López cumple años el 2 de marzo"/>
    </div>
    <div class="title footer">
      <p class="footer_letters">
      {{ footer }}
      </p>
      <img class="footer_icon" src="../assets/arrow.png"/>
      </div>
  </div>
</template>

<script>
import childBirthdateCard from "./childComponents/childBirthdateCard"
export default {
  name: 'birthdateCard',
  props: {
    header: String,
    footer:String,
  },
  components:{
    childBirthdateCard,
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
.bodyBirthdate {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);
  grid-gap:3px;
  background-color: rgba(235,239,242, 0.2);
  padding-top:0.5em;
  overflow: hidden;
}
</style>