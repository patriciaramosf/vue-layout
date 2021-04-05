<template>
  <div class="child childPayrollCard">
    <div class="payroll__row">
      <p class="payroll__description">{{ payRollDescription }}</p>
      <img class="payroll__image" src="../../assets/box.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: "childPayrollCard",
  props: {
    payRollDescription: String,
  },
};
</script>
<style>
.childPayrollCard {
  font-size: 14px;
  background: white;
  padding: 5px;
}
.payroll__row {
  position: relative;
  display: flex;
  align-items: center;
  text-align: left;
  padding: 5px;
}
.payroll__description {
  width: 80%;
}
.payroll__image {
  width: 20px;
  position: absolute;
  right: 10px;
}
</style>