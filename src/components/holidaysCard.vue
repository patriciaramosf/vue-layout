<template>
  <div class="item holidaysWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyHolidays">
      <childHolidaysCard
        holidaysDate="San José"
        holidaysMonth="Mar"
        holidaysDay="13"
        holidaysLocation="En Madrid, Barcelona y 3 más"
        holidaysDayOfWeek="miércoles"
      />
      <childHolidaysCard
        holidaysDate="San Ignacio de Loyola"
        holidaysMonth="Mar"
        holidaysDay="30"
        holidaysLocation="En Madrid, Barcelona y 3 más"
        holidaysDayOfWeek="viernes"
      />
      <childHolidaysCard
        holidaysDate="Mi festivo 1"
        holidaysMonth="Abr"
        holidaysDay="02"
        holidaysLocation="En Barcelona"
        holidaysDayOfWeek="domingo"
      />
      <childHolidaysCard
        holidaysDate="Mi festivo 2"
        holidaysMonth="Ago"
        holidaysDay="17"
        holidaysLocation="En Madrid"
        holidaysDayOfWeek="miércoles"
      />
       <childHolidaysCard
        holidaysDate="San José"
        holidaysMonth="Mar"
        holidaysDay="13"
        holidaysLocation="En Barcelona"
        holidaysDayOfWeek="lunes"
      />
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
import childHolidaysCard from "./childComponents/childHolidaysCard";
export default {
  name: "holidaysCard",
  props: {
    header: String,
    footer: String,
  },
  components: {
    childHolidaysCard,
  },
};
</script>
<style>
.holidaysWrapper {
  grid-column-start: 1;
  grid-column-end: 5;
  grid-row-start: 5;
  grid-row-end: 9;
}
.bodyHolidays {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(3, 1fr);
  grid-gap:8px;
  background-color: rgba(235,239,242, 0.2);
  padding-top:0.5em;
  overflow: hidden;
}
</style>