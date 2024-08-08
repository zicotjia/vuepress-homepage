<template>
 <div class="text-with-logo">
    <div v-if="image" class="logo-content">
      <img :src="$withBase(image)" alt="" class="logo">
    </div>
    <div class="text-content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ['image']
};
</script>

<style lang="stylus">

@import './styles/config.styl';

.text-with-logo {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
}

.text-content {
  flex: 1;
}

.logo-content {
  margin-right: 20px;
  max-width: 50px !important; /* Adjust as needed */
  height: auto;
}

</style>