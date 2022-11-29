<template>
  <header class="header" z-40>
    <nuxt-link to="/" w-10 h-10 absolute lg:fixed m-6 select-none outline-none>
      <img src="~/assets/img/logo.png" alt="logo" />
    </nuxt-link>
    <nav class="nav">
      <div class="space" />
      <div class="right">
        <nuxt-link title="Blog" to="/blogs" decoration-none>
          <span lt-md:hidden>Blog</span>
        </nuxt-link>
        <nuxt-link title="Blog" to="/blogs" decoration-none>
          <span lt-md:hidden>Projects</span>
        </nuxt-link>
        <nuxt-link title="Blog" to="/blogs" decoration-none>
          <span lt-md:hidden>About</span>
        </nuxt-link>
        <a
          i-carbon-logo-github
          href="https://github.com/franklin23"
          target="_blank"
          lt-md:hidden
        />
        <a
          i-carbon-logo-twitter
          href="https://twitter.com/znmkp123"
          target="_blank"
          lt-md:hidden
        />
        <toggle-theme />
      </div>
    </nav>
  </header>
</template>

<style scoped>
  .header {
    margin-bottom: 0;
  }

  .nav {
    padding: 2rem;
    width: 100%;
    display: grid;
    grid-template-columns: auto max-content;
    box-sizing: border-box;
  }
  .nav > * {
    margin: auto;
  }
  .nav .right {
    display: grid;
    grid-gap: 1.2rem;
    grid-auto-flow: column;
  }
</style>
