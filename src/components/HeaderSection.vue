<script lang="ts" setup>
enum constants {
  EMAIL = 'contact@sortilege-onglerie.ch',
}
</script>

<template>
  <div class="header-section">
    <img src="@/assets/icon.png" alt="icon" class="icon" />
    <h1>Sortilège onglerie</h1>
    <span class="swiss-quality">
      Qualité suisse
      <img src="@/assets/swiss-flag.webp" alt="swiss-flag" class="swiss-flag" />
    </span>
    <a :href="`mailto:${constants.EMAIL}`" class="email">
      {{ constants.EMAIL }}
    </a>
    <img class="cat" src="@/assets/cat.png" alt="cat" />
  </div>
</template>

<style lang="scss" scoped>
.header-section {
  background-color: #f8f8f8;
  padding: 5px 20px 20px 20px;
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 30px;
  position: relative;
  text-align: center;

  .icon {
    width: 200px;
    margin-bottom: 20px;
  }

  h1 {
    font-size: 2.5em;
    margin: 0;
  }

  .swiss-quality {
    display: flex;
    align-items: center;
    gap: 10px;
    font-size: 1rem;
    font-weight: 500;

    .swiss-flag {
      width: 20px;
    }
  }

  .email {
    font-size: 1em;
    font-weight: 500;
    cursor: pointer;
    user-select: none;
    transition: all 200ms ease;
    color: #333333;

    &:hover {
      opacity: 0.5;
      text-decoration: underline;
    }
  }

  .cat {
    position: absolute;
    bottom: -14px;
    right: 20%;
    width: 120px;
  }
}
</style>
