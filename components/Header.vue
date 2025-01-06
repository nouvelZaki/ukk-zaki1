<template>
<nav class="navbar navbar-expand-lg bg-body-tertiary  m-2 " style="padding-left: 32%;">
  <img src="~/assets/smk.png" alt="Bootstrap"  width="30" height="30">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">SMKN 4 TASIKMALAYA</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0 pt-2">
        <nuxt-link to="/">
            <li class="nav-item">
              <h6>HOME</h6>
            </li>
        </nuxt-link>
        <li class="nav-item dropdown ms-2">
        </li>
          <nuxt-link to="/profile">
            <li class="nav-item">
              <h6>PROFILE</h6>
            </li>
          </nuxt-link>
          <li class="nav-item dropdown ms-2">
        </li>
          <nuxt-link to="/eskul">
            <li class="nav-item">
              <h6>EKSTRAKULIKULER</h6>
            </li>
          </nuxt-link>
      <li class="nav-item dropdown ms-2">
        </li>
          <nuxt-link to="/galeri">
            <li class="nav-item">
              <h6>GALERI</h6>
            </li>
          </nuxt-link>
      </ul>
    </div>
  </div>
</nav>
</template>