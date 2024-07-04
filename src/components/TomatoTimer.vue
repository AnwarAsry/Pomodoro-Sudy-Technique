<script setup lang="ts"></script>

<template>
  <div class="tomato">
    <div class="red">
      <div class="time-display">
        <span id="minutes">00</span>
        :
        <span id="seconds">00</span>
      </div>
    </div>
    <div class="green">
      <div class="leaves"></div>
      <div class="leaves"></div>
      <div class="leaves"></div>
      <div class="leaves"></div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.time-display {
  width: 100%;
  position: absolute;
  bottom: 70px;
  text-align: center;
  font-size: 5rem;
}

.tomato {
  position: relative;
}

.tomato .red {
  width: 340px;
  height: 270px;
  position: relative;
  border-radius: 55% 55% 60% 60%;
  background-color: rgb(248, 71, 40);
}

.tomato .green::before {
  content: '';
  position: absolute;
  inset: -45px 170px;
  width: 20px;
  height: 90px;
  border-radius: 70% 70% 0% 0%;
  background-color: rgb(12, 165, 4);
  transform: rotateZ(10deg);
}

.leaves {
  position: absolute;
  width: 0;
  height: 0;
  border-right: 20px solid transparent;
  border-top: 80px solid rgb(12, 165, 4);
  border-left: 20px solid transparent;
}

.leaves:nth-child(1) {
  inset: -30px 110px;
  transform: rotateZ(120deg);
}

.leaves:nth-child(2) {
  inset: 20px 120px;
  transform: rotateZ(40deg);
}

.leaves:nth-child(3) {
  inset: 20px 185px;
  transform: rotateZ(-50deg);
}

.leaves:nth-child(4) {
  inset: -30px 190px;
  transform: rotateZ(-120deg);
}
</style>
