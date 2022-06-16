<template>
  <NavBar></NavBar>
  <PrincipalMain></PrincipalMain>
  <FooterComponent></FooterComponent>
  <div class="BOXA" v-if="selected === 'SOLO'">
    <OffreChoice
      :titleOffre="'SOLO *'"
      :textOffre1a="'1 ECRAN VIDEO HD'"
      :textOffre1b="'9,99 € / MOIS'"
      :contenu="'* ACCES ILLIMITÉ A PLUS DE 1000 FILMS ET SERIES'"
    >
      <button class="button1" @click="selectOffer('null')">RETOUR</button>
    </OffreChoice>
  </div>
  <div class="BOXB" v-if="selected === 'FAMILY'">
    <OffreChoice
      :titleOffre="'FAMILY *'"
      :textOffre1a="'4 ECRANS VIDEO HD'"
      :textOffre1b="'12,99 € / MOIS'"
      :contenu="'* ACCES ILLIMITÉ A PLUS DE 1000 FILMS ET SERIES'"
    >
      <button class="button2" @click="selectOffer('null')">RETOUR</button>
    </OffreChoice>
  </div>
  <div class="BOXC" v-if="selected === 'FAMILY 4K'">
    <OffreChoice
      :titleOffre="'FAMILY 4K *'"
      :textOffre1a="'4 ECRAN VIDEO 4K'"
      :textOffre1b="'15,99 € / MOIS'"
      :contenu="'* ACCES ILLIMITÉ A PLUS DE 1000 FILMS ET SERIES'"
    >
      <button class="button3" @click="selectOffer('null')">RETOUR</button>
    </OffreChoice>
  </div>

  <div class="BOX" v-if="selected === 'null'">
    <PrincipalMain2
      :title="`SOLO`"
      :text1="`1 ECRAN VIDEO HD`"
      :text2="`9,99 € / MOIS`"
    >
      <button @click="selectOffer('SOLO')">S'ABONNER</button>
    </PrincipalMain2>
    <PrincipalMain2
      :title="`FAMILY`"
      :text1="`4 ECRANS VIDEO HD`"
      :text2="`12,99 € / MOIS`"
    >
      <button @click="selectOffer('FAMILY')">S'ABONNER</button></PrincipalMain2
    >
    <PrincipalMain2
      :title="`FAMILY 4K`"
      :text1="`4 ECRANS VIDEO 4K`"
      :text2="`15,99 € / MOIS`"
      ><button @click="selectOffer('FAMILY 4K')">
        S'ABONNER
      </button></PrincipalMain2
    >
  </div>
</template>

<script>
import NavBar from "./components/NavBar";
import PrincipalMain from "./components/PrincipalMain";
import FooterComponent from "./components/FooterComponent";
import PrincipalMain2 from "./components/PrincipalMain2";
import OffreChoice from "./components/OffreChoice";

export default {
  name: "App",
  data() {
    return {
      selected: "null",
    };
  },
  methods: {
    selectOffer: function (offer) {
      this.selected = offer;
    },
    // comeBack: function (offer) {
    //   this.selected = offer;
    // },
  },
  components: {
    NavBar,
    PrincipalMain,
    FooterComponent,
    PrincipalMain2,
    OffreChoice,
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  height: 100vh;
  background-image: linear-gradient(to top, #fddb92 0%, #d1fdff 100%);
}

.BOX {
  display: flex;
  justify-content: center;
}

button {
  color: rgb(18, 111, 219);
  font-weight: 700;
}

.button1 {
  width: 100px;
  margin-left: 300px;
  margin-top: 20px;
  color: rgb(18, 111, 219);
  font-weight: 700;
}

.button2 {
  width: 100px;
  margin-left: 300px;
  margin-top: 20px;
  color: rgb(18, 111, 219);
}

.button3 {
  width: 100px;
  margin-left: 300px;
  margin-top: 20px;
  color: rgb(18, 111, 219);
}
</style>
