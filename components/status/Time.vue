<template>
  <v-col>
    <Clock
      v-for="time in times"
      :key="time.name"
      :name="time.name"
      :time="time.time"
    ></Clock>
  </v-col>
</template>

<script>
import Clock from '~/components/status/Time/Clock'

export default {
  name: 'Time',
  components: {
    Clock,
  },
  data() {
    return {
      timezones: [
        {
          name: 'UTC',
          offset: 0,
        },
        {
          name: 'MDT (UTC-06)',
          offset: -6,
        },
        {
          name: 'PDT (UTC-07)',
          offset: -7,
        },
        {
          name: 'EDT (UTC-04)',
          offset: -4,
        },
      ],
      times: [],
    }
  },
  mounted() {
    this.$options.timer = window.setTimeout(this.updateTimes, 1000)
  },
  methods: {
    updateTimes() {
      this.times = this.timezones.map((timezone) => {
        return {
          name: timezone.name,
          time: this.computeTime(timezone.offset),
        }
      })
      this.$options.timer = window.setTimeout(this.updateTimes, 1000)
    },
    computeTime(offset) {
      const now = new Date()
      const yr = now.getUTCFullYear()
      const month = now.getUTCMonth()
      const day = now.getUTCDay()
      const hr = now.getUTCHours()
      const min = now.getUTCMinutes()
      const sec = now.getUTCSeconds()
      return new Date(yr, month, day, hr + offset, min, sec)
    },
  },
}
</script>

<style scoped></style>
