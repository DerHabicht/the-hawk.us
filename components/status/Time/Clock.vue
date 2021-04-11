<template>
  <v-row>
    <v-col>
      <v-card>
        <v-card-title>{{ name }}</v-card-title>
        <v-card-text>
          <div class="clock">
            {{ _time }}
          </div>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import dateformat from 'dateformat'

export default {
  name: 'Clock',
  props: {
    name: {
      type: String,
      default: 'UTC',
    },
    time: {
      type: Date,
      default: new Date(),
    },
  },
  computed: {
    _time() {
      return dateformat(this.time, 'HH:MM:ss')
    },
  },
}
</script>

<style scoped>
.clock {
  font-size: x-large;
}
</style>
