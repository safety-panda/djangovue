<template>
  <br>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <paragraph-comp :texty="paragraphText"></paragraph-comp>
  </div>
  <br>
</template>

<script>
import ParagraphComp from "./ParagraphComp.vue"

export default {
  components: { ParagraphComp },
  name: 'HelloWorld',
  data: function() {
    return {
      elsa: "Princess Elsa",
      anna: "Princess Anna",
    };
  },
  props: {
    msg: String,
  },
  computed: {
    paragraphText: function () {
      let text;
      text = "Arendelle has two princesses: " + this.elsa + " and " + this.anna
      return text
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #314E70;
}
</style>
