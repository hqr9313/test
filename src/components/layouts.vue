<template>
  <div class="container">
    <nav>
      <HqrHeader :msg="webName" />
    </nav>
    <section>
      <div><LeftBody /></div>
      <div></div>
    </section>
    <footer></footer>
  </div>
</template>

<script>
import HqrHeader from "./header/HqrHeader";
import LeftBody from "./body/LeftBody";
export default {
  components: {
    HqrHeader,
    LeftBody,
  },
  data() {
    return {
      webName: "我是标题",
    };
  },
  watch: {},
  methods: {},
  mounted() {},
};
</script>
  
<style scoped>
nav {
  width: 100%;
  height: 120px;
  border: 1px solid blue;
}
footer {
  width: 100%;
  height: 120px;
  border: 1px solid blue;
}

section {
  display: flex;
  justify-content: space-between;
}
section div {
  width: 50%;
  height: 400px;
}
section div:nth-child(1) {
  border: 1px solid red;
}
section div:nth-child(2) {
  border: 1px solid burlywood;
}
</style>