<template> <!-- ici je créé un input date basique -->
  <div class="temp d-f">
    <label for="Date">select a date </label>
    <input type="date" name="date" id="date" required />
  </div>
</template>

<script>
export default {
  name: "DateInput",
  props: {
    msg: String,
  },
};
</script>

<style>

</style>