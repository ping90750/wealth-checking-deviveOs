<template>
  <div id="app">
    <a
      href="https://play.google.com/store/apps/details?id=capital.dcone.wallet"
    >
      <img src="./assets/android.png" class="buttonImg" />
    </a>
    <a href="https://apps.apple.com/th/app/dc-one/id1529399567">
      <img src="./assets/ios.png" class="buttonImg" />
    </a>
  </div>
</template>

<script>
export default {
  name: "App",
  created() {
    if (navigator.userAgent.toLowerCase().indexOf("android") > -1) {
      window.location.href =
        "https://play.google.com/store/apps/details?id=capital.dcone.wallet";
    }
    if (navigator.userAgent.toLowerCase().indexOf("iphone") > -1) {
      window.location.href =
        "https://apps.apple.com/th/app/dc-one/id1529399567";
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.buttonImg {
  width: 150px;
  height: 80px;
}
</style>
