<template>
  <main class="main">
    <div class="down2">
      <div class="left">
        <h3>{{ title }}</h3>
        <p class="para">{{ text1 }}</p>
        <p>{{ text2 }}</p>
        <slot />
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainPrincipal2",
  props: {
    title: String,
    text1: String,
    text2: String,
  },
};
</script>

<style>
.down2 {
  height: 200px;
  display: flex;
  justify-content: space-evenly;
  margin-left: 25%;
  margin-top: 50px;
}

.left {
  background-color: rgb(18, 111, 219);
  border-radius: 5px;
  height: 220px;
  width: 250px;
  color: white;
  text-align: center;
}

.para {
  width: 100px;
  text-align: center;
  margin-left: 40px;
}
</style>
