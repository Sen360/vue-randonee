<template>
  <div>
    <v-carousel class="caroussel" :show-arrows="false">
      <v-carousel-item src="../assets/foret.jpg">
        <v-btn x-large class="button"> Découvrez des randonées inédites </v-btn>
      </v-carousel-item>
      <v-carousel-item src="../assets/automne.jpg"> </v-carousel-item>
    </v-carousel>
  </div>
</template>

<style>
.caroussel {
    margin-bottom: 100px;
}
.button {
    background-color: green !important;
    margin-top: 180px;
}
</style>
