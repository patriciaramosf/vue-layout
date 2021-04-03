<template>
  <div class="item exitWrapper">
    <div class="title header">
      <h1 class="header_letters">{{ header.toUpperCase() }}</h1>
    </div>
    <div class="body bodyExit">
      <h2 class="text__secondary">No hay salidas próximas</h2>
      <img class="exitIcon" src="../assets/face-monocle.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: "exitsCard",
  props: {
    header: String,
  },
};
</script>
<style>
.exitWrapper {
  grid-column-start: 10;
  grid-column-end: 13;
  grid-row-start: 1;
  grid-row-end: 3;
}
.bodyExit {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.exitIcon {
  width: 30px;
  height: 30px;
}
</style>