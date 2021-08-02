<template>
  <button @click="Onclick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  },
  methods: {
    Onclick() {
      this.$emit('btn-click')
    },
  },
}
</script>

<style>
</style>