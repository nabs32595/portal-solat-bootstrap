<template>
  <div>
    <b-container>
      <b-card class="my-5">
        <b-row>
          <b-col>
            <b-table
              responsive
              :items="prayerTime"
              :fields="fields"
              :tbody-tr-class="rowClass"
            >
              <template #cell(date)="data">
                {{ data.item.date }}
              </template>

              <template #cell(subuh)="data">
                {{ $moment(data.item.fajr, 'HH:mm:ss').format('LT') }}
              </template>

              <template #cell(zohor)="data">
                {{ $moment(data.item.dhuhr, 'HH:mm:ss').format('LT') }}
              </template>

              <template #cell(asar)="data">
                {{ $moment(data.item.asr, 'HH:mm:ss').format('LT') }}
              </template>

              <template #cell(magrib)="data">
                {{ $moment(data.item.maghrib, 'HH:mm:ss').format('LT') }}
              </template>

              <template #cell(isyak)="data">
                {{ $moment(data.item.isha, 'HH:mm:ss').format('LT') }}
              </template>
            </b-table>
          </b-col>
        </b-row>
      </b-card>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      prayerTime: [],
      fields: [
        { key: 'date', label: 'Date' },
        { key: 'subuh', label: 'Subuh' },
        { key: 'zohor', label: 'Zohor' },
        { key: 'asar', label: 'Asar' },
        { key: 'magrib', label: 'Maghrib' },
        { key: 'isyak', label: 'Isyak' },
      ],
    }
  },
  mounted() {
    this.getPrayerTime()
  },
  methods: {
    rowClass(item, type) {
      if (!item || type !== 'row') return
      if (item.date === this.$moment().format('DD-MMM-YYYY'))
        return 'table-info'
    },
    async getPrayerTime() {
      const res = await this.$axios.$get(
        'https://www.e-solat.gov.my/index.php?r=esolatApi/takwimsolat&period=month&zone=SGR01'
      )
      this.prayerTime = res.prayerTime
    },
  },
}
</script>

<style scoped></style>
