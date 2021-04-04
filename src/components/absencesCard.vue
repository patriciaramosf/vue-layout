<template>
  <div class="item absencesWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyAbsences">
      <childAbsencesCard
        absencesDescription="Paula Palmera"
        absencesImage="sickness.png"
        absencesType="Baja médica"
        absencesDates="25/03/2021 de 10.03 a 11.23"
      />
    <childAbsencesCard
        absencesDescription="Paula Palmera"
        absencesImage="vacation.png"
        absencesType="Vacaciones"
        absencesDates="25/03/2021 de 10.03 a 11.23"
      />
      <childAbsencesCard
        absencesDescription="Paula Palmera"
        absencesImage="absence.png"
        absencesType="Ausencia"
        absencesDates="25/03/2021 de 10.03 a 11.23"
      />
      <childAbsencesCard
        absencesDescription="Paula Palmera"
        absencesImage="vacation.png"
        absencesType="Baja médica"
        absencesDates="25/03/2021 de 10.03 a 11.23"
      />
      <childAbsencesCard
        absencesDescription="Paula Palmera"
        absencesImage="sickness.png"
        absencesType="Baja médica"
        absencesDates="25/03/2021 de 10.03 a 11.23"
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
import childAbsencesCard from "./childComponents/childAbsencesCard";
export default {
  name: "absencesCard",
  props: {
    header: String,
    footer: String,
  },
  components: {
    childAbsencesCard,
  },
};
</script>
<style>
.absencesWrapper {
  grid-column-start: 1;
  grid-column-end: 5;
  grid-row-start: 1;
  grid-row-end: 5;
}
.bodyAbsences {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-template-rows: auto;
  grid-gap: 5px;
  overflow: hidden;
  padding-top:0.5em;
}
</style>