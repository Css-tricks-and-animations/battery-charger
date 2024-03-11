<template>
  <BatteryCharger />
</template>

<script>
import BatteryCharger from "./components/BatteryCharger.vue";

export default {
  name: "App",
  components: {
    BatteryCharger,
  },
};
</script>

<style>
#app {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: #0b0c0d;
}
</style>
