<template>
  <progress class="progress" :value="newValue" max="100"></progress>
</template>

<script>
export default {
  name: 'Progress',
  props: {
    value: {
      type: Number,
      default: 0
    },
    duration: {
      type: Number,
      default: 500
    }
  },
  data() {
    return {
      newValue: 0,
      step: 0
    }
  },
  watch: {
    value() {
      this.growInit()
    }
  },
  mounted() {
    this.growInit()
  },
  methods: {
    growInit() {
      let m = this.value / (this.duration / 25)
      this.grow(m)
    },
    grow(m) {
      let v = Math.ceil(this.newValue + m)

      if (v > this.value) {
        this.newValue = this.value
        return false
      }

      this.newValue = v
      setTimeout(() => {
        this.grow(m)
      }, 25)
    }
  }
}
</script>

