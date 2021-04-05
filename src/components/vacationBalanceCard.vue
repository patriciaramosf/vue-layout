<template>
  <div class="item vacationWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyVacation">
      <img class="exitIcon" src="../assets/vacation.png" />
      <div class="vacationTitle">
        <p class="text_vacation_h2">23 dias</p>
        <p class="text_vacation_p">Total de 24 dias</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "vacationBalanceCard",
  props: {
    header: String,
  },
};
</script>
<style>
.vacationWrapper {
  grid-column-start: 5;
  grid-column-end: 8;
  grid-row-start: 5;
  grid-row-end: 7;
}
.bodyVacation {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  padding: 5px;
  text-align: left;
}
.vacationTitle {
  display: flex;
  flex-direction: column;
  position: relative;
  text-align: left;
  padding-left:0.5em;
  margin-top:10%;
}
.text_vacation_h2{
  margin:0;
  font-weight:700;
  font-size:30px;
}
.text_vacation_p{
margin-top:0px;
}
</style>