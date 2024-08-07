<template>
  <div class="md-card" :class="{ 'show-border': !hideBorder}">
    <div v-if="videoSrc" class="card-image">
      <video :src="$withBase(videoSrc)" controls></video>
    </div>
    <div class="card-content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ['videoSrc', 'hideBorder']
};
</script>

<style lang="stylus">
@import './styles/config.styl';

.md-card
  background-color $cardColor
  margin-top 1.5em
  min-height 225px
  display flex
  flex-direction row
  align-items stretch

  .card-image
    flex: 0 0 20%
    display flex
    align-items center
    justify-content center
    padding 0.75rem
    video 
      max-width 100%
      max-height 100%
      width auto
      height auto
      border 1px solid #eee
      border-radius 0.2rem
      object-fit cover

  .card-content
    flex: 1
    padding 0.75rem
    display flex
    flex-direction column
    justify-content center
    p
      line-height normal
      -webkit-margin-before 0em
      -webkit-margin-after 0.75em
    blockquote 
      font-size 1.5rem

.md-card.show-border
  border 1px solid #eee
  border-radius 0.5rem
  box-shadow 0 5px 15px -5px rgba(0,0,0,.1)
  padding 0.75rem

@media (max-width: $MQMobileNarrow)
  .md-card
    display flex
    flex-direction column
    margin 1.5rem -0.75rem
    padding 0.75rem
    box-sizing border-box

    .card-image
      flex-grow 1
      align-items stretch
      video 
        width 100%
        max-width 600px

    .card-content
      pre
        margin 0
        border-radius 6px

</style>
