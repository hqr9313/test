<template>
  <div class="">
    <ul>
      <li @click="goPage"><a href="#" />{{ username }}</li>
      <li><a href="#" />菜单12</li>
      <li><a href="#" />菜单13</li>
      <li><a href="#" />{{ count }}</li>
      <li><a href="#" />{{ counts }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: "admin",
      count: 1,
    };
  },
  methods: {
    goPage() {
      console.log(1232131);
      this.username = "hahah";
    },
  },
  computed: {
    counts() {
      return this.count + 100;
    },
  },
};
</script>

<style>
li:hover {
  color: red;
}
</style>