<script setup lang="ts"></script>

<template>
  <div class="shortcuts" id="mode_timer">
    <button class="shortcuts__slide" id="tabpomo">Pomodoro</button>
    <button class="shortcuts__slide" id="shortbreak">Short Break</button>
    <button class="shortcuts__slide" id="longbreak">Long Break</button>
  </div>
</template>

<style scoped lang="scss">
.shortcuts {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  gap: 20px;

  &__slide {
    cursor: pointer;
    width: fit-content;
    height: 40px;
    padding: 0 20px;
    border: none;
    border-radius: 10px;
    box-shadow: 0 5px 10px black;
    font-size: 1rem;
    font-weight: 600;
    background-color: rgb(12, 165, 4);
    transition: all 200ms ease-in-out;

    &:hover {
      background-color: rgba(69, 240, 60, 0.806);
    }
  }
}
</style>
