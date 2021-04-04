<template>
  <div class="child childAbsencesCard">
    <div class="absences__row">
      <div class="childAbsencesCard_dateCartoon">
        <img
          class="childAbsencesCard_dateCartoon__image"
          :src="require(`@/assets/${absencesImage}`)"
        />
      </div>
      <div>
        <p class="absences__description">{{ absencesDescription }}</p>
        <div class="absences__type_wrapper">
          <div :style="{ backgroundColor: activeColor}" class="absences__type_circle"></div>
          <p class="absences__type_name" :style="{ color: activeColor}">{{ absencesType }}</p>
        </div>
      </div>
      <p class="absences__dates">{{ absencesDates }}</p>
      <img class="absences__image" src="../../assets/arrow.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: "childAbsencesCard",
  props: {
    absencesDescription: String,
    absencesImage: String,
    absencesType: String,
    absencesDates: String,
  },
};
</script>
<style>
.childAbsencesCard {
  font-size: 12px;
  background: white;
  padding: 5px;
}
.absences__row {
  position: relative;
  display: flex;
  align-items: center;
  text-align: left;
  padding: 5px;
  padding-right: 12px;
  justify-content: space-around;
}
.childAbsencesCard_dateCartoon {
  border-radius: 50%;
  width: 35px;
  height: 35px;
  border: none;
  display: flex;
  flex-direction: column;
  background-color: rgba(235, 239, 242);
  align-items: center;
  justify-content: center;
  position: relative;
}
.childAbsencesCard_dateCartoon__image {
  width: 30px;
}
.absences__type_wrapper {
  display: flex;
  align-items: center;
  position: relative;
  bottom: 18px;
  text-align:left;
}
.absences__description {
  font-size: 12px;
  font-weight: 700;
   text-align: left;
}
.absences__type_name{
  text-align: left;
}
.absences__type_circle {
  border-radius: 50%;
  width: 10px;
  height: 10px;
  border: none;
  margin-right: 2px;
}
.absences__image {
  width: 8px;
  height: 14px;
  position: absolute;
  right: 10px;
}
.absences__dates{
   color:darkgrey;
  font-weight:200;
}
</style>