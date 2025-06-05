<script lang="ts" setup>
import GiftImage from '@/assets/phoneGifts.jpg'

const emit = defineEmits<{
  (e: 'onClick'): void
}>()
</script>
<template>
  <div class="token-section">
    <div class="text-content">
      <h1>Your Customized Token<br />For Globally Compliant<br />Distribution Events</h1>
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
      <button class="get-started" @click="emit('onClick')">Get Started</button>
    </div>
    <div class="graphic">
      <img :src="GiftImage" alt="Token Graphic" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.token-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(to right, #1a1aff, #00bfff);
  padding: 3rem;
  color: #fff;
  font-family: 'Arial', sans-serif;
  flex-wrap: wrap;

  .text-content {
    max-width: 500px;

    h1 {
      font-size: 2.5rem;
      line-height: 1.4;
      margin-bottom: 1rem;
    }

    p {
      font-size: 1rem;
      margin-bottom: 2rem;
    }

    .get-started {
      background-color: #00e6e6;
      color: #000;
      border: none;
      padding: 0.8rem 1.5rem;
      border-radius: 30px;
      font-weight: bold;
      cursor: pointer;

      &:hover {
        background-color: #00cccc;
      }
    }
  }

  .graphic {
    flex: 1;
    text-align: center;

    img {
      max-width: 100%;
      height: auto;
    }
  }
}
</style>
