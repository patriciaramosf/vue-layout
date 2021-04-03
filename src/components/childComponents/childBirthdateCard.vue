<template>
  <div class="child childBirthdateCard">
    <div class="childBirthdateCard_dateCartoon">
      <img class="user__image" src="../../assets/user.png" />
      <div class="childBirthdateCard_dateCartoon_second">
        <img class="birthdate__image" src="../../assets/birthday.png" />
      </div>
    </div>
    <p class="birthdate__description">{{ birthdateDescription }}</p>
  </div>
</template>

<script>
export default {
  name: "childBirthdateCard",
  props: {
    birthdateDescription: String,
  },
};
</script>
<style>
.childBirthdateCard {
  font-size: 12px;
  background: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding:5px;
}
.childBirthdateCard_dateCartoon {
  border-radius: 50%;
  width: 55px;
  height: 55px;
  border: none;
  display: flex;
  flex-direction: column;
  background-color: #f57c05;
  align-items: center;
  justify-content: center;
  position: relative;
}
.childBirthdateCard_dateCartoon_second {
  border-radius: 50%;
  width: 30px;
  height: 30px;
  overflow: hidden;
  border: none;
  display: flex;
  flex-direction: column;
  background-color: rgba(235,239,242);
  align-items: center;
  justify-content: center;
  position: absolute;
  left: 30px;
  top: 30px;
}
.user__image {
  width: 30px;
}
.birthdate__image {
  width: 10px;
}
</style>