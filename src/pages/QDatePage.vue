<template>
    <!-- <div class="q-pa-md">
    <div class="q-pb-sm">
      Model: {{ days }}
    </div>

    <q-date v-model="days" multiple />
  </div> -->
  <qdate></qdate>
</template>

<script>
import { ref } from 'vue'
// 1
// import QDate from 'components/QDate.vue'

export default {
  components: {
    // 1
    // 'qdate': QDate
    // 2
    'qdate': require('components/QDate.vue').default
  },
    setup () {
        return {
        days: ref([ '2019/02/01', '2019/02/10' ])
        }
    }
}
</script>

<style>

</style>