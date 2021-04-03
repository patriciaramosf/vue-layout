<template>
  <div class="item holidaysWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyHolidays">
      <div class="rowHolidays">
        <childHolidaysCard
          holidaysDate="San José"
          holidaysMonth="Mar"
          holidaysDay="13"
          holidaysLocation="En Madrid, Barcelona y 3 más"
        />
        <childHolidaysCard
          holidaysDate="San José"
          holidaysMonth="Mar"
          holidaysDay="13"
          holidaysLocation="En Barcelona"
        />
      </div>
      <div class="rowHolidays">
        <childHolidaysCard
          holidaysDate="San José"
          holidaysMonth="Mar"
          holidaysDay="13"
          holidaysLocation="En Madrid, Barcelona y 3 más"
        />
        <childHolidaysCard
          holidaysDate="San José"
          holidaysMonth="Mar"
          holidaysDay="13"
          holidaysLocation="En Barcelona"
        />
      </div>
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
  display: flex;
  flex-direction: column;
  align-items:center;
  justify-content: center;
}
.rowHolidays {
  display: flex;
  flex-direction: row;
}
</style>