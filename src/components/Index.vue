<template>
  <div>
    <div class="header">
      <h1>This is header</h1>
    </div>
    <Body />
  </div>
</template>
<script>
import Body from "./Body";
export default {
  name: "Index",
  components: {
    Body,
  },
};
</script>
<style>
div.header {
  background-color: cadetblue;
  height: 80px;
  padding: 20px;
}
</style>