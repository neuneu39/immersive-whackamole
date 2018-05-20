<template>
  <div class="moles-container">
    <div class="mole" 
      v-for="(mole, index) in moleData" 
      v-bind:key="index"
      >
      {{mole}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'Moles',
  props: [ 'moleData' ]
}
</script>

<style>

</style>

