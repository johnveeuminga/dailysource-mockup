<template>
  <header class="header">
    <div class="container">
      <img src="@/assets/header.jpg" alt="Header Placeholder">
    </div>
    <nav id='nav' class='navbar bg-secondary'>
      <div class="container">
        <div class="navbar__wrapper">
          <ul class='navbar__nav nav'>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                Home
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                About Us
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                Our Team
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                Volunteer
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                Ways To Help
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class='nav-link'>
                News Archives
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to='#' class="nav-link">
                Opinion
              </router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'TheHeader'
}
</script>

<style lang="scss" scoped>
.header {
  img {
    max-width: 100%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
}

.navbar {
  padding-top: 0;
  padding-bottom: 0;

  &__wrapper {
    width: 100%;
  }

  &__nav {
    width: 100%;
  }

  .nav-item {
    flex-grow: 1;
    flex-shrink: 1;
    text-align: center;
    margin-top: 0.5rem;
    margin-bottom: 0.5rem;

    &:not(:last-child) {
      border-right: 1px solid #fff;
    }
  }

  .nav-link {
    display: inline-block;
    color: #fff;
    font-weight: 700;
    padding-top: 0;
    padding-bottom: 0;
  }
}
</style>
