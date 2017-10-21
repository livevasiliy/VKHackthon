<template>
  <v-card height="57px">
    <v-bottom-nav
      absolute
      shift
      :value="true"
      :active.sync="e2"
      :class="{
        'blue-grey': e2 === 1,
        'teal': e2 === 2,
        'brown': e2 === 3,
        'brown lighten-1': e2 === 4
      }"
    >
      <v-btn dark>
        <span>Подробнее</span>
        <v-icon>info</v-icon>
      </v-btn>
      <v-btn dark>
        <span>Пойду</span>
        <v-icon>directions_walk
</v-icon>
      </v-btn>
      <v-btn dark>
        <span>Найти</span>
        <v-icon>search</v-icon>
      </v-btn>
    </v-bottom-nav>
  </v-card>
</template>



<script>
  export default {
    data () {
      return {
        e2: 3
      }
    }
  }
</script>

