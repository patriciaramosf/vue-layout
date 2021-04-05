<template>
  <div class="item payRollWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body payRollBody">
      <childPayRollCard payRollDescription="Nómina de febrero - 2021" />
      <childPayRollCard payRollDescription="Nómina de enero - 2021" />
      <childPayRollCard payRollDescription="Nómina de abril - 2021" />
      <childPayRollCard
        payRollDescription="Certificado de retenciones de enero - 2021"
      />
      <childPayRollCard payRollDescription="Nómina de febrero - 2021" />
      <childPayRollCard payRollDescription="Nómina de febrero - 2021" />
    </div>
    <div class="title footer">
      <p class="footer_letters">
        {{ footer }}
      </p>
      <img class="footer_icon" src="../assets/arrow.png" />
    </div>
  </div>
</template>

<script>
import childPayRollCard from "./childComponents/childPayRollCard";
export default {
  name: "payRollCard",
  props: {
    header: String,
    footer: String,
  },
  components: {
    childPayRollCard,
  },
};
</script>
<style>
.payRollWrapper {
  grid-column-start: 10;
  grid-column-end: 13;
  grid-row-start: 3;
  grid-row-end: 7;
}
.payRollBody {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-template-rows: auto;
  grid-gap: 5px;
  overflow: hidden;
  padding-top: 0.5em;
}
</style>