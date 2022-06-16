<template>
  <footer class="footer">
    <h3 class="titleFooter">NETPRIME+</h3>
    <p class="paraFooter">&copy; Tous droits réservés</p>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style>
.footer {
  background-color: rgb(18, 111, 219);
  height: 100px;
  width: 100%;
  display: flex;
}

.titleFooter {
  width: 25%;
  color: white;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: 500;
  font-size: x-large;
  display: flex;
  justify-content: center;
  align-items: center;
}

.paraFooter {
  width: 40%;
  color: white;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: 200;
  font-size: small;
  display: flex;
  justify-content: center;
  align-items: flex-end;
}
</style>
