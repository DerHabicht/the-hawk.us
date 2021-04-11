<template>
  <v-row>
    <v-col>
      <v-img
        src="lair-herriman_emblem.png"
        max-height="200"
        max-width="200"
        contain
      ></v-img>
    </v-col>
    <v-col align="center">
      <div class="header">
        Lair Herriman <br />
        {{ today }}
      </div>
    </v-col>
    <v-spacer></v-spacer>
  </v-row>
</template>

<script>
import dateformat from 'dateformat'

export default {
  name: 'StatusTitleBar',
  computed: {
    today() {
      const d = new Date()
      return dateformat(d, 'dddd dd mmmm yyyy')
    },
  },
}
</script>

<style scoped>
.header {
  font-size: xxx-large;
}
</style>
