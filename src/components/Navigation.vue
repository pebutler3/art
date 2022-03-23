<template>
  <nav>
    <ul>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<style>
ul {
  background-color: black;
  list-style: none;
  margin: 0;
  padding: 0;
}

li {
  display: flex;
}

li a {
  color: white;
  font-weight: bold;
  padding: 2rem 2rem;
  text-decoration: none;
  text-transform: uppercase;
}

li a:hover {
  background-color: pink;
  color: black;
}
</style>
