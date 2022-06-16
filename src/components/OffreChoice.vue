<template>
  <div class="BOX4">
    <h3 class="titleOffre">{{ titleOffre }}</h3>
    <p class="textOffre1a">{{ textOffre1a }}</p>
    <p class="textOffre1b">{{ textOffre1b }}</p>
    <p class="contenu">{{ contenu }}</p>
    <slot />
    <!-- <button class="buttonBack" @click="window.scrollY">RETOUR</button> -->
  </div>
</template>

<script>
export default {
  name: "OffreChoice",
  props: ["titleOffre", "textOffre1a", "textOffre1b", "contenu"],
};
</script>

<style>
.BOX4 {
  background-color: rgb(18, 111, 219);
  border-radius: 5px;
  height: 400px;
  width: 50%;
  text-align: center;
  display: flex;
  flex-direction: column;
  margin-top: 30px;
  margin-left: 25%;
}

.titleOffre {
  color: white;
  font-size: xx-large;
  border: 2px white solid;
  width: 350px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 25%;
}

.textOffre1a {
  color: white;
  font-size: x-large;
}

.textOffre1b {
  color: white;
  font-size: x-large;
}

.contenu {
  color: white;
  font-size: large;
  font-family: monospace;
}

.buttonBack {
  width: 300px;
  height: 30px;
  border-radius: 5px;
  background-color: whitesmoke;
  color: rgb(18, 111, 219);
  font-size: large;
  font-weight: 600;
  font-family: monospace;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 30%;
}

/* main {
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
} */
</style>
