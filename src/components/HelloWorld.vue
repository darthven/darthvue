<template>
  <v-container>
    <v-layout>
      <v-flex>
        <div class="hello">
          <h1>{{ msg }}</h1>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HelloWorld',
  props: {
    msg: String,
  },
})
</script>
