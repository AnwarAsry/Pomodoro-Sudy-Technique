<script setup lang="ts">
import TomatoTimer from './components/TomatoTimer.vue'
import TimerSettings from './components/TimerSettings.vue'
import TimerShortcuts from './components/TimerShortcuts.vue'
import TimerControl from './components/TimerControl.vue'
</script>

<template>
  <div class="container">
    <div class="wrapper">
      <TimerShortcuts></TimerShortcuts>
      <TomatoTimer></TomatoTimer>
      <TimerControl></TimerControl>
    </div>
    <TimerSettings></TimerSettings>
  </div>
</template>

<style scoped lang="scss">
.container {
  width: 700px;
  min-height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 70px;

  .wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 70px;
  }
}
</style>
