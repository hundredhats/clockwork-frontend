<template>
  <header>
    <h1>Like Clockwork</h1>
    <nav>
      <a href="/login"><li>Login</li></a>
      <a href="/signup"><li>Signup</li></a>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>
header {
  box-sizing: border-box;
  padding: 20px;
}

h1 {
  display: inline-block;
  width: 40%;
  font-size: 1em;
  margin: 0;
}

nav {
  text-align: right;
  display: inline-block;
  width: 59%;
}

li {
  display: inline-block;
  list-style: none;
  padding: 0 10px;
}

a {
  text-decoration: none;
  color: #2c3e50;
}
</style>
