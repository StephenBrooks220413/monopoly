<template>
  <div id="nav">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <router-link class="navbar-brand" to="/">CodeSchool</router-link>
        <button
          class="navbar-toggler"
          type="button"
          data-mdb-toggle="collapse"
          data-mdb-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <i class="fas fa-bars"></i>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/previous"
                >Previous</router-link
              >
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/upcoming"
                >Upcoming</router-link
              >
            </li>
            <!-- Dropdown -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                id="navbarDropdownMenuLink"
                role="button"
                data-mdb-toggle="dropdown"
                aria-expanded="false"
              >
                Courses
              </a>
              <ul
                class="dropdown-menu"
                aria-labelledby="navbarDropdownMenuLink"
              >
                <li><a class="dropdown-item" href="#">Basics</a></li>
                <li><a class="dropdown-item" href="#">Vue.js</a></li>
                <li>
                  <a class="dropdown-item" href="#">React.js</a>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </nav>
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
