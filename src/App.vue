<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view />
</template>

<script>
import * as mdb from "mdb-ui-kit";

export default {
  mdb,
};
</script>

<style lang="scss">
@import "~mdb-ui-kit/css/mdb.min.css";
@import "./assets/navbar.scss";
@import "./assets/main.scss";
@import "./assets/board.scss";
@import "./assets/player.scss";
@import "./assets/styles.scss";
</style>
