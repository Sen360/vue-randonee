<template>
  <div>
    <ul class="card">
      <v-container>
        <v-row>
          <li v-for="card in cards" :key="card.message">
            <v-col>
              <v-card>
                <v-img
                  class="white--text align-end"
                  height="200px"
                  :src="card.image"
                  width="300px"
                >
                  <v-card-title>{{ card.title }}</v-card-title>
                </v-img>

                <v-card-subtitle class="pb-0">
                  {{ card.title }}
                </v-card-subtitle>

                <v-card-text class="text--primary">
                  <div>Whitehaven Beach</div>

                  <div>Whitsunday Island, Whitsunday Islands</div>
                </v-card-text>

                <v-card-actions>
                  <v-btn color="orange" text> Share </v-btn>

                  <v-btn color="orange" text> Explore </v-btn>
                </v-card-actions>
              </v-card>
            </v-col>
          </li>
        </v-row>
      </v-container>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Body",
  data() {
    return {
      cards: [
        { title: "Randonnée 1", image: require("../assets/montagne.jpg") },
        { title: "Randonné 2", image: require("../assets/alpinisme.jpg") },
        { title: "Randonée 3", image: require("../assets/conemarra.jpg") },
        { title: "Randonée 4", image: require("../assets/japonais.jpg") },
        { title: "Randonée 5", image: require("../assets/banc.jpg") },
        { title: "Randonée 6", image: require("../assets/lake.jpg") },
        { title: "Randonée 7", image: require("../assets/traversee.jpg") },
        { title: "Randonée 8", image: require("../assets/dolomite.jpg") },
        { title: "Randonée 9", image: require("../assets/mer.jpg") },
      ],
    };
  },
};
</script>

<style>
.card {
    margin-top: 250px;
    margin-bottom: 60px;
    list-style-type: none;
    background-color: #006400;
}
</style>
