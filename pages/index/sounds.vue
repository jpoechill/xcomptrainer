<template>
    <div class="container py-2">
      <div class="row">
        <div v-for="n in 9" :key="n" class="col-md-4 my-3">
          <div @click="playSound('0' + n)" :class="(n%2 === 0) ? ['bg-blue', 'ripple-drk'] : ['bg-light', 'ripple-lgt', 'text-dark']" class="tab noselect text-center text-uppercase p-2 rounded font-weight-bold">
            Sound {{ n }}
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  mounted() {
    window.addEventListener('keydown', this.handleKeys, true)
  },
  beforeDestroy(){
    window.removeEventListener('keydown', this.handleKeys, true)
  },
  computed: {
    handleColor: function (n) {
      if (n) {
        return true;
      }
    }
  },
  methods: {
    playSound: function (soundIndex) {
      var soundFile = "/kill-sound-" + soundIndex + ".mp3"
      var audio = new Audio(soundFile)

      audio.play();
    },
    handleKeys: function (event) {
      switch (event.key) {
        case 'q':
          this.playSound('01')
          break;
        case 'w':
          this.playSound('02')
          break;
        case 'e':
          this.playSound('03')
          break;
        case 'r':
          this.playSound('04')
          break;
        case 't':
          this.playSound('05')
          break;
        case 'y':
          this.playSound('06')
          break;
        case 'u':
          this.playSound('07')
          break;
        case 'i':
          this.playSound('08')
          break;
        case 'o':
          this.playSound('09')
          break;
      }
    }
  },
}
</script>

<style>

</style>