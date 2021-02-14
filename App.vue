<template>
  <view class="container">
    <HeaderTest />
    <text class="text-color-primary">{{ message }}</text>
    <button title="Press me!" @press="exclaim" />
  </view>
</template>

<script>
import HeaderTest from "./HeaderTest";

export default {
  components: { HeaderTest },
  data() {
    return {
      message: "Hello World"
    };
  },
  methods: {
    exclaim() {
      this.message += "!";
    }
  },
};
</script>

<style>
.container {
  flex: 1;
  background-color: white;
  align-items: center;
  justify-content: center;
}
.text-color-primary {
  color: blue;
  font-size: 30px;
}
</style>
