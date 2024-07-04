<script setup lang="ts"></script>

<template>
  <div class="timer-settings">
    <button class="button" id="plusmin">+1m</button>
    <button class="button" id="plusthirty">+30s</button>
    <button class="button" id="plussec">+1s</button>
    <button class="button-reset" id="reset">Reset</button>
  </div>
</template>

<style scoped lang="scss">
.timer-settings {
  width: fit-content;
  height: fit-content;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;

  button {
    cursor: pointer;
    height: 80px;
    width: 80px;
    border: none;
    border-radius: 100%;
    box-shadow: 0 5px 10px black;
    font-size: 1.3rem;
    background-color: rgb(248, 71, 40);
    transition: all 200ms ease-in-out;

    &:hover {
      background-color: rgb(255, 97, 69);
    }
  }

  .button-reset {
    height: 40px;
    font-size: 1rem;
    font-weight: 600;
    border-radius: 10px;
  }
}
</style>
