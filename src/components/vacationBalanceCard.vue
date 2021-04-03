<template>
  <div class="item vacationWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyVacation">
      <div class="vacationTitle">
      <img class="exitIcon" src="../assets/vacation.png" />
        <h2 class="text_vacation_h2">23 dias</h2>
      </div>
        <p>total de 24 dias</p>
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
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.vacationTitle {
  display:flex;
  justify-content: center;
  align-items: center;
  margin-bottom:-1.2em;/* review */
}
</style>