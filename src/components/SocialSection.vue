<script lang="ts" setup>
enum constants {
  INSTAGRAM = 'https://www.instagram.com/sortilegeonglerie/',
  FACEBOOK = 'https://www.facebook.com/profile.php?id=100090384391532',
}

const openSocial = (url: string) => window.open(url, '_blank');
</script>

<template>
  <div class="social">
    <i class="pi pi-instagram" @click="openSocial(constants.INSTAGRAM)" />
    <i class="pi pi-facebook" @click="openSocial(constants.FACEBOOK)" />
  </div>
</template>

<style scoped lang="scss">
.social {
  display: flex;
  gap: 20px;
  font-size: 1.4rem;
  margin: 50px 0 0 0;
  justify-content: center;

  i {
    cursor: pointer;
    user-select: none;
    transition: all 200ms ease;

    &:hover {
      opacity: 0.5;
    }
  }
}
</style>
