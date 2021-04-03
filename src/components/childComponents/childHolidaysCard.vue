<template>
  <div class="child childHolidaysCard">
    <h2 class="childHolidaysCard_date">{{ holidaysDate }}</h2>
    <div class="childHolidaysCard_dateCartoon">
      <div class="month_date">
        {{ holidaysMonth }}
      </div>
      <div class="day_date">
        {{ holidaysDay }}
      </div>
    </div>
    <p class="childHolidaysCard_location text__secondary">
      {{ holidaysLocation }}
    </p>
  </div>
</template>

<script>
export default {
  name: "childHolidaysCard",
  props: {
    holidaysDate: String,
    holidaysMonth: String,
    holidaysDay: String,
    holidaysLocation: String,
  },
};
</script>
<style>
.childHolidaysCard {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.childHolidaysCard_date {
  font-size: 14px;
}
.childHolidaysCard_dateCartoon {
  border-radius: 50%;
  border: 1px solid grey;
  width: 50px;
  height: 50px;
  background-color: #ebeff2;
}
.month_date {
  background-color: #f57c05;
  color: white;
  shape-outside: circle(50% at 50% 50%);
}
.day_date {
    shape-outside: circle(50% at 50% 50%);
}
</style>