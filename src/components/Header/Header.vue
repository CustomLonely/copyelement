<template>
  <mt-header :title="mytitle">
    <mt-button @click="goPage()" icon="back" slot="left"></mt-button>
  </mt-header>
</template>

<script>
export default {
  props: ["mytitle"],
  data() {
    return {};
  },
  created() {
    console.log(this.mytitle);
  },
  mounted() {
    console.log(this.mytitle);
  },
  methods: {
    goPage() {
      this.$router.go(-1);
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>
