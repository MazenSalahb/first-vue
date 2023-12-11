<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="container">
    <div class="col-8 mx-auto">
      <nav
        class="navbar navbar-expand-lg bg-body-tertiary rounded mt-4 mb-5 shadow"
      >
        <div class="container-fluid">
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarTogglerDemo01"
            aria-controls="navbarTogglerDemo01"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
            <a class="navbar-brand" href="#">Mazengo</a>
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <RouterLink class="nav-link active" aria-current="page" to="/"
                  >Home</RouterLink
                >
              </li>
              <li class="nav-item">
                <RouterLink class="nav-link" to="/profile">Profile</RouterLink>
              </li>
              <li class="nav-item">
                <a class="nav-link disabled" aria-disabled="true">Disabled</a>
              </li>
            </ul>
            <div class="d-flex gap-2">
              <button type="button" class="btn btn-outline-success">
                Login
              </button>
              <button type="button" class="btn btn-outline-success">
                Register
              </button>
            </div>
          </div>
        </div>
      </nav>

      <!-- Pages -->
      <RouterView />
    </div>
  </div>
</template>

<style scoped></style>
