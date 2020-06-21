<template>
  <div class="container">
    <div>
      <div v-for="report in reports" :key="report.id">
        {{ report.id }}
        {{ report.todaysConfirmed }}
      </div>
    </div>
  </div>
</template>

<script>

  export default {
    components: {
    },
    data() {
      return {
        reports: [
          {
            id: 1,
            todaysConfirmed: 1,
            recovered: 55,
            active: {
              count: 38,
              created: "2020-03-03T18:25:43.511Z"
            },
            totalConfirmed: 94,
            tested: 5900,
            deaths: 1,
            worldwide: {
              count: 4508435,
              created: "2020-03-03T18:25:43.511Z"
            },
            gender: {
              male: 1,
              female: 1,
              created: "2020-03-03T18:25:43.511Z"
            },
            age: {
              start: 14,
              end: 85,
              created: "2020-03-03T18:25:43.511Z"
            },
            severity: {
              asymptomatic: 29,
              symptomatic: 9,
              created: "2020-03-03T18:25:43.511Z"
            },
            hospital: {
              hospitalized: 0,
              nonHospitalized: 38,
              created: "2020-03-03T18:25:43.511Z"
            },
            isolation: {
              count: 163,
              created: "2020-03-03T18:25:43.511Z"
            },
            created: "2020-03-03T18:25:43.511Z",
            author: 1
          }
        ]
      }
    }
  }
</script>

<style>
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }
</style>
