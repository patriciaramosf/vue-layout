<template>
  <div class="child childHolidaysCard">
    <h2 class="childHolidaysCard_date">{{ holidaysDate }}</h2>
    <div class="childHolidaysCard_dateCartoon">
      <div class="month_date">
        {{ holidaysMonth.toLowerCase() }}
      </div>
      <div class="wrapperDates">
        <p class="day_dateWeek">{{ holidaysDayOfWeek.toUpperCase() }}</p>
        <p class="day_date">{{ holidaysDay }}</p>
      </div>
    </div>
    <p class="childHolidaysCard_location">
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
    holidaysDayOfWeek:String,
  },
};
</script>
<style>
.childHolidaysCard {
  font-size: 10px;
  background: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding:5px;
}
.childHolidaysCard_date{
  font-size:12px;
}
.childHolidaysCard_dateCartoon {
  border-radius: 50%;
  width: 55px;
  height: 55px;
  overflow: hidden;
  border: none;
  display: flex;
  flex-direction: column;
}
.month_date {
  background-color: #f57c05;
  color: white;
  text-align: center;
  font-size: 14px;
  padding: 2px;
}
.wrapperDates{
 background-color: #ebeff2;
 text-align: center;
 display:flex;
 flex-direction: column;
justify-content: center;
}
.day_date {
  font-weight: 700;
  font-size: 14px;
  position: relative;
  bottom: 18px;
}
.day_dateWeek{
  font-size:6px;
}
</style>