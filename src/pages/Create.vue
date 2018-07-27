<template lang="html">
  <div class="create">
    <h5>Create</h5>
    <div class="create__box">
      <div class="create__box__game">
        <ImageSpeech/>
      </div>
      <div class="create__box__form">

      </div>
    </div>
  </div>
</template>

<script>
import ImageSpeech from '@/components/ImageSpeech'

export default {
  name: 'Create',
  components: {
    ImageSpeech
  }
}
</script>

<style lang="scss">
  .create {
    height: 100%;
    font-size: 3rem;
    h5 {
      text-align: center;
    }
    &__box {
      height: 100%;
      display: grid;
      grid-template-rows: 1fr 1fr;
    }
  }
</style>
