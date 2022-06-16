<template>
  <nav class="nav">
    <h1 class="titleNav">NETPRIME+</h1>
    <p class="paraNav">La plateforme video complètement originale</p>
  </nav>
</template>

<script>
export default {
  name: "NavBarPrincipal",
};
</script>

<style>
.nav {
  margin-top: 20px;
  background-color: rgb(18, 111, 219);
  height: 100px;
  width: 100%;
  display: flex;
}

.titleNav {
  width: 25%;
  color: white;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: 900;
  font-size: xx-large;
  display: flex;
  justify-content: center;
}

.paraNav {
  width: 75%;
  color: white;
  font-family: Verdana, Geneva, Tahoma, sans-serif;

  font-weight: 700;
  font-size: large;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
