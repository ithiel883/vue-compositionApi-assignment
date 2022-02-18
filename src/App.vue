<template>
  <h2>{{courseGoal}}</h2>
  <!-- Task 1: Output your main course goal with help of the composition API -->
  <!-- Don't hardcode it into the template, instead hardcode it into the JS code -->
  <h3>OUTPUT COURSE GOAL</h3>
  <!-- Task 2: Toggle (show/ hide) the goal with help of the button  -->
  <button @click="toggleGoal">Toggle Goal</button>
  <!-- Task 3: Manage data in three ways -->
  <!-- => Separate refs -->
  <!-- => Ref Object -->
  <!-- => Reactive Object -->
  <!-- Task 4: Also solve the assignment with the Options API -->
</template>

<script>
  import { ref } from 'vue';

export default {

  setup(){
      const goal = ref('master vue')

  const aims = ref({
    goal: 'eat Vue'
  })
  const moreGoals = 
      function changeGoal(){
          goal.value = 'Live and Breath Vue'
      }

return {
courseGoal: goal,
toggleGoal: changeGoal
}
  }
}
</script>

<style>
html {
  font-family: sans-serif;
}
body {
  margin: 3rem;
  text-align: center;
}
</style>