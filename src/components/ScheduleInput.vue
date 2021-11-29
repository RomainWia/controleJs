<template>
  <div class="temp">
    <p>Choose one of the available timeslots</p>

    <div v-for="item in items" :key="item.schedule" class="tt" > <!-- ici je créé ma boucle pour avoir tout mes inputs avec les données de mes items -->
        <div class="{{item.premium}} {{item.prime}}"> <!-- je cherche a ajouter une classe premium et prime pour les éléments qui en ont pour ajouter une couleur au css  -->
            <input type="radio" id="{{item.schedule}}" name="schedule" value="{{item.schedule}}" required /> 
            <label for="{{item.schedule}}">{{item.schedule}}</label>
        </div>
        
    </div>
    <!--
    <div class="inline">
      <input type="radio" id="12h00" name="schedule" value="12h00" required />
      <label for="12h00">12h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="12h30" name="schedule" value="12h30"  />
      <label for="12h30">12h30</label>
    </div>
    <div class="inline">
      <input type="radio" id="13h00" name="schedule" value="13h00"  />
      <label for="13h00">13h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="13h30" name="schedule" value="13h30"  />
      <label for="13h30">13h30</label>
    </div>
    <div class="inline">
      <input type="radio" id="14h00" name="schedule" value="14h00"  />
      <label for="14h00">14h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="14h30" name="schedule" value="14h30"  />
      <label for="14h30">14h30</label>
    </div>
    <div class="inline">
      <input type="radio" id="15h00" name="schedule" value="15h00"  />
      <label for="15h00">15h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="15h30" name="schedule" value="15h30"  />
      <label for="15h30">15h30</label>
    </div>
    <div class="inline">
      <input type="radio" id="16h00" name="schedule" value="16h00"  />
      <label for="16h00">16h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="18h00" name="schedule" value="18h00"  />
      <label for="18h00">18h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="18h30" name="schedule" value="18h30"  />
      <label for="18h30">18h30</label>
    </div>
    <div class="inline">
      <input type="radio" id="19h00" name="schedule" value="19h00"  />
      <label for="19h00">19h00</label>
    </div>
    <div class="inline">
      <input type="radio" id="19h30" name="schedule" value="19h30"  />
      <label for="19h30">19h30</label>
    </div> -->
  </div>
</template>

<script>
export default {
  name: "ScheduleInput",
  props: {
    msg: String,
  },

  data() {
    return {
      items: [
          {schedule: '12h00', premium : 'no', prime: 'no'},
          {schedule: '12h30', premium : 'no', prime: 'no'},
          {schedule: '13h00', premium : 'no', prime: 'no'},
          {schedule: '13h30', premium : 'no', prime: 'no'},
          {schedule: '14h00', premium : 'no', prime: 'yesprime'},
          {schedule: '14h30', premium : 'no', prime: 'yesprime'},
          {schedule: '15h00', premium : 'no', prime: 'yesprime'},
          {schedule: '15h30', premium : 'no', prime: 'no'},
          {schedule: '16h00', premium : 'no', prime: 'no'},
          {schedule: '18h00', premium : 'yespremium', prime: 'no'},
          {schedule: '18h30', premium : 'yespremium', prime: 'no'},
          {schedule: '19h00', premium : 'yespremium', prime: 'no'},
          {schedule: '19h30', premium : 'yespremium', prime: 'no'}
      ]
    }
  },
};
</script>

<style>

</style>