<template>
  <v-card height="57px">
    <v-bottom-nav absolute :value="true" :active.sync="e1" class="transparent">
      <v-btn flat color="teal" value="recent">
        <span>Подробнее</span>
        <v-icon>info</v-icon>
      </v-btn>
      <v-btn flat color="teal" value="favorites">
        <span>Пойду</span>
        <v-icon>directions_walk</v-icon>
      </v-btn>
      <v-btn flat color="teal" value="nearby">
        <span>Найти</span>
        <v-icon>place</v-icon>
      </v-btn>
    </v-bottom-nav>
  </v-card>
</template>



<script>
  export default {
    data () {
      return {
        e1: 'recent'
      }
    }
  }
</script>
