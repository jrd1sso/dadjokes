<template>
  <header class="header">
    <h2 class="title">Dad Jokes</h2>

    <ul>
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>

      <li>
        <nuxt-link to="/jokes">Jokes</nuxt-link>
      </li>

      <li>
        <nuxt-link :to="{ name: 'about' }">About</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {};
</script>

<style>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
  border-bottom: 1px dotted #ccc;
}

.header .title {
  font-size: 1.75rem;
  color: #526488;
}

.header ul {
  display: flex;
}

.header a {
  display: inline-block;
  background: #9e8f8f;
  color: #fff;
  padding: 0.3rem 1rem;
  margin-right: 0.5rem;
}

.header .nuxt-link-exact-active {
  background: #526488;
}
</style>
