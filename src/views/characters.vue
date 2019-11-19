<template>
  <div>
    <br />
    <div class="container">
      <div class="row">
        <div class="col-sm" v-for="character in characters" :key="character.id">
          <div>
            <b-card
              v-bind:title="character.name"
              :img-src="character.url"
              img-alt="Image"
              img-top
              tag="article"
              style="max-width: 20rem;"
              class="mb-2"
            >
              <b-card-text>{{character.description}}</b-card-text>

              <b-button @click="ok" variant="primary">Go somewhere</b-button>
            </b-card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Json from '../db.json';
export default {
  name: "Characters",
  data() {
    return {
      characters: Json.characters
    };
  },
  methods: {
    ok() {
        alert();
    }
  }
};
</script>