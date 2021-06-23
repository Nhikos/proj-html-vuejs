<template>
  <div class="infobox">
    <h6>{{info.via}}</h6>
    <h6>{{info.city}}</h6>
    <h6>{{info.telephone}}</h6>
  </div>
</template>

<script>
export default {
    name: "Infobox",
    props: {
        info: Object,
    }
}
</script>

<style scoped>
.infobox {
    display: flex;
    flex-direction: column;
    color: white;
    height: 86px;
    width: 250px;
}
h6 {
  color: #a7a7a7;
  font-size: 14px;
}
</style>