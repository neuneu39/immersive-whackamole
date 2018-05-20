<template>
  <div class="whackmole">
    <div class="logo">Whack-a-mole!</div>
    <button class="game-start" v-on:click="gameStart">Start Round</button>
    <div class="counters-container">
      <div class="counter">
        <h1>Whacks:</h1>
        <h2>{{ score }}</h2>
      </div>
      <div class="counter">
        <h1>High Score:</h1>
        <h2>{{ highScore }}</h2>
      </div>
      <div class="counter">
        <h1>TIMER:</h1>
        <h2>{{ timer }}</h2>
      </div>
    </div>
    <div class="moles-container">
      <div class="mole">{{ mole[0] }}</div>
      <div class="mole">{{ mole[1] }}</div>
      <div class="mole">{{ mole[2] }}</div>
      <div class="mole">{{ mole[3] }}</div>
    </div>
  </div>

</template>

<script>
export default {
  data: () => {
    return {
      score: 3,
      highScore: 15,
      timer: 0,
      mole: [ false, false, false, false ]
    };
  },
  methods: {
    gameStart: () => {
      alert('ok!');
    },
  }
  
}
</script>

<style>
.counter {
  margin: 10px;
  display: inline-block;
}
.mole {
  margin: 10px;
  display: inline-block;
}

</style>
