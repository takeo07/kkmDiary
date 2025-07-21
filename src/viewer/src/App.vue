<template>
  <v-app>
    <v-main>
      <VCalendar :events="events"/>
    </v-main>
  </v-app>
</template>

<script lang="ts" setup>
import { ref } from 'vue';
import { VCalendar } from 'vuetify/labs/VCalendar';

const events = ref([
  {
    title: 'Meeting with Team',
    start: new Date('2025-07-22'),
    end: new Date('2025-07-22'),
    color: 'blue',
  },
  {
    title: 'Project Deadline',
    start: new Date('2025-07-25'),
    end: new Date('2025-07-25'),
    color: 'red',
  },
  {
    title: 'Conference',
    start: new Date('2025-07-28'),
    end: new Date('2025-07-29'),
    color: 'green',
  },
]);
</script>
