<template>
  <navbar></navbar>
  <library></library>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Library from "./components/Library.vue";

export default {
  components: {
    Navbar,
    Library
  },
};
</script>

<style>
:root {
  --background-clr: #d9e7e5;
  --secondary-background-clr: #d9e7e5;
  --hover-clr: #d7f6f4;
  --accent-clr: #f9b5aa;
  --secondary-accend-clr: #f2cac5;
  --accent-hover-clr: #f89a90;
  --dark-text-clr: #333333;
  --secondary-dark-text-clr: #555555;
  --text-clr: #ffffff;
  --secondary-text-clr: #cccccc;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  height: 100vh;
  font-family: Arial, sans-serif;
  background-color: var(--background-clr);
  color: var(--dark-text-clr);
}

.header {
  width: 100%;
  height: 4rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
}

.nav {
  display: flex;
  gap: 15px;
  margin: 1rem;
}

.nav a {
  background-color: var(--accent-clr);
  text-decoration: none;
  color: var(--text-clr);
  font-size: 1rem;
  font-weight: bold;
  padding: 0.5rem 1.5rem;
  border-radius: 2rem;
}

.nav a:hover {
  background-color: var(--accent-hover-clr);
}

.search {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.search input {
  border: 1px solid var(--secondary-text-clr);
  border-radius: 2rem;
  padding: 0.75rem;
}

.btn {
  background-color: var(--accent-clr);
  color: var(--text-clr);
  border: none;
  border-radius: 2rem;
  padding: 0.5rem 1.5rem;
  cursor: pointer;
  font-size: 1rem;
  font-weight: bold;
}

.btn:hover {
  background-color: var(--accent-hover-clr);
}
</style>