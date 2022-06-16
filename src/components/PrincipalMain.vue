<template>
  <main class="main">
    <div class="top">
      <h5 class="titleMain1">NOS FORMULES D'ABONNEMENT</h5>
      <p class="paraMain1">
        Toutes nos formules d'abonnement sont 100% sans
        <br />
        <br />
        engagement et résiliables à tout moment. Paiement par <br />
        <br />
        CB, Paypal et en BitCoin possible.
      </p>
    </div>
    <div class="down">
      <h4 class="titleMain2">DECOUVREZ TRÈS BIENTÔT NOS OFFRES</h4>
      <p class="paraMain2">A PARTIR DE 9,99€ / MOIS</p>
      <button class="button" @click="handleShowbanner">EN SAVOIR PLUS</button>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainPrincipal",
  data() {
    return {
      showBanner: false,
    };
  },
  methods: {
    handleShowbanner: function () {
      this.showBanner = !this.showBanner;
    },
  },
};
</script>

<style>
main {
  height: 550px;
  margin-bottom: 20px;
  display: flex;
  flex-direction: column;
}

.top {
  width: 400px;
  margin-top: 20px;
  margin-left: 80px;
}

.titleMain1 {
  font-family: monospace;
  font-size: large;
  font-weight: 300;
  color: rgb(18, 111, 219);
}

.paraMain1 {
  font-family: monospace;
  font-size: small;
  font-weight: 100;
  text-align: justify;
}

.down {
  background-color: rgb(18, 111, 219);
  height: 200px;
  width: 50%;
  border-radius: 5px;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: auto;
  color: white;
}

.titleMain2 {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-size: x-large;
  font-weight: 400;
}

.paraMain2 {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-size: medium;
  font-weight: 200;
}

.button {
  width: 400px;
  height: 30px;
  border-radius: 5px;
  background-color: white;
  color: rgb(18, 111, 219);
  font-family: monospace;
  font-size: 200;
  font-weight: 600;
  margin: auto;
}
</style>
