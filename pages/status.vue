<template>
  <div>
    <StatusTitleBar></StatusTitleBar>
    <v-row>
      <Time></Time>
      <Weather></Weather>
      <Calendar></Calendar>
    </v-row>
  </div>
</template>

<script>
import Calendar from '~/components/status/Calendar'
import StatusTitleBar from '~/components/status/StatusTitleBar'
import Time from '~/components/status/Time'
import Weather from '~/components/status/Weather'

export default {
  name: 'Status',
  components: {
    Calendar,
    StatusTitleBar,
    Time,
    Weather,
  },
}
</script>

<style scoped></style>
