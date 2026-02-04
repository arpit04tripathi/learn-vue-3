<template>
  <header class="bg-gradient bg-light p-2 border-bottom border-dark border-3">
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <!-- Bootstrap 5 Navbar image and text https://getbootstrap.com/docs/5.3/components/navbar/#image-and-text -->
        <RouterLink class="navbar-brand" to="/">
          <img src="@/assets/logo.svg" alt="Logo" width="30" height="24" class="d-inline-block align-text-top">
          Vue 3
        </RouterLink>
        <!-- <a class="navbar-brand" href="#">
          <img src="@/assets/logo.svg" alt="Logo" width="30" height="24" class="d-inline-block align-text-top">
          Vue 3
        </a> -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <RouterLink class="nav-link" to="/">
                <span><i class="bi bi-house-door-fill"></i> Home</span>
              </RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link p-2" to="/about">About</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link p-2" to="/bootstrap">Bootstrap</RouterLink>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="https://vuejs.org/examples/#hello-world" target="_blank"
                role="button" data-bs-toggle="dropdown" aria-expanded="false">
                Examples
              </a>
              <ul class="dropdown-menu">
                <li>
                  <RouterLink class="nav-link p-2 mx-2" to="/default">Default Vue</RouterLink>
                </li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li>
                  <hr class="dropdown-divider">
                </li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link disabled" to="/default" aria-disabled="true">Disabled</RouterLink>
            </li>
          </ul>
        </div>

      </div>
    </nav>
  </header>
</template>
