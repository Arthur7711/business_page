<script setup lang="ts">
import TeamImage from '@/assets/team.jpg'
</script>

<template>
  <div class="hero-section">
    <section class="main-content">
      <div class="text-section">
        <h1 class="title">BUSINESS</h1>
        <p class="description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
          ut labore et dolore magna aliqua erat volutpat.
        </p>
        <button class="search-btn">SEARCH</button>
      </div>
      <div class="image-section">
        <img :src="TeamImage" alt="Team" />
      </div>
    </section>
  </div>
</template>

<style lang="scss" scoped>
.hero-section {
  background: linear-gradient(to right, #3a2ff2, #251c93);
  color: #fff;
  font-family: 'Arial', sans-serif;
  padding: 2rem;

  .main-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;

    .text-section {
      flex: 1;
      max-width: 500px;

      .title {
        font-size: 4rem;
        margin-bottom: 1rem;
      }

      .description {
        font-size: 1rem;
        margin-bottom: 2rem;
        color: #f0eeee;
      }

      .search-btn {
        background-color: white;
        color: #3a2ff2;
        border: none;
        padding: 1rem 2rem;
        border-radius: 30px;
        font-weight: bold;
        cursor: pointer;

        &:hover {
          background-color: #ddd;
        }
      }
    }

    .image-section {
      flex: 1;
      text-align: center;

      img {
        max-width: 100%;
        height: auto;
      }
    }
  }
}
</style>
