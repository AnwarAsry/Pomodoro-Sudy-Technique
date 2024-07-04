<script setup lang="ts"></script>

<template>
  <div class="controls">
    <button class="slide" id="playpause">Play</button>
  </div>
</template>

<style scoped lang="scss">
.controls {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  gap: 20px;

  button {
    cursor: pointer;
    width: fit-content;
    height: 40px;
    padding: 0 20px;
    border: none;
    border-radius: 10px;
    font-size: 1rem;
    font-weight: 600;
    box-shadow: 0 5px 10px black;
    background-color: rgb(12, 165, 4);
    transition: all 200ms ease-in-out;

    &:hover {
      background-color: rgba(69, 240, 60, 0.806);
    }
  }
}
</style>
