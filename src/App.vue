<template>
  <form action="" method="" class="d-f">
    <DateInput msg="" />
    <ScheduleInput msg=""  />
    <Button msg="" v-on:validation="valide=true" />
    <Informations msg="" />
    <div v-if="valide === true ">
      <p>reservation registered</p>
    </div>
    <div v-if="valide !== true ">
      <p>reservation not registered yet</p>
    </div>
  </form>
</template>

<script>

import DateInput from "./components/DateInput.vue";
import ScheduleInput from "./components/ScheduleInput.vue";
import Button from "./components/Button.vue";
import Informations from "./components/Informations.vue";


export default {
  name: 'App',
  components: {
    DateInput,
    ScheduleInput,
    Button,
    Informations
  },
  data() {
    return {
      valide: false
    }
  },
}
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
  color: grey;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
.tt {
  margin-top: 10px;
}
.tt2 {
  margin-top: 30px;
}
.d-f {
  display:flexbox;
}
</style>
