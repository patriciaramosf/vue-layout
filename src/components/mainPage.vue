<template>
  <div class="wrapper">
    <absencesCard />
    <birthdateCard />
    <exitsCard />
    <holidaysCard />
    <payRollCard />
    <vacationBalanceCard />
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.wrapper {
  width:90%;
  height:100vh;
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(9, 1fr);
  grid-gap: 20px;
  border:1px solid black;
}
.item{
  border:solid red
}
</style>
