<template>
  <div class="wrapper">
    <absencesCard header="próximas ausencias" footer="Ver todas" />
    <birthdateCard header="próximos cumpleaños" footer="Ir al calendario" />
    <exitsCard header="próximas salidas" />
    <holidaysCard header="próximos festivos" footer="Ir al calendario" />
    <payRollCard header="últimas nóminas" footer="Ver todas" />
    <vacationBalanceCard header="saldo de vacaciones" />
  </div>
</template>

<script>
import absencesCard from "./absencesCard";
import birthdateCard from "./birthdateCard";
import exitsCard from "./exitsCard";
import holidaysCard from "./holidaysCard";
import payRollCard from "./payRollCard";
import vacationBalanceCard from "./vacationBalanceCard";
export default {
  name: "mainPage",
  props: {
    msg: String,
  },
  components: {
    absencesCard,
    birthdateCard,
    exitsCard,
    holidaysCard,
    payRollCard,
    vacationBalanceCard,
  },
};
</script>
<style>
.wrapper {
  width: 90%;
  height: 100vh;
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(9, 1fr);
  grid-gap: 20px;
}
.item {
  border-top: solid #f57c05 4px;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
  align-items: center;
}
.title {
  width: 100%;
  text-align: center;
  box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.2);
  font-weight: 700;
}
/* header css */
.header_letters {
  font-size: 16px;
  padding: 10px;
}
.body {
  background-color: rgba(235, 239, 242, 0.3);
  width: 100%;
  height: 100%;
}
/* footer css */
.footer {
  color: #f57c05;
  display: flex;
  justify-content: center;
  align-items: center;
}
.footer_letters {
  font-weight: 500;
  font-size: 16px;
}
.footer_icon {
  width: 8px;
  height: 14px;
  padding-left: 5px;
}
</style>
