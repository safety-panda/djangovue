<template>
  <div class="para">
    <p><b>{{ texty }}</b></p>
  </div>
</template>

<script>
export default {
  name: 'ParagraphComp',
  props: {
    texty: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  color: #F582A8;
}
</style>
