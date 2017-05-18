<template>
  <div class="flowchart-container top-circle">
    <section class="flowchart">
      <div class="flowchart-block" v-for="flowchart in flowcharts">
        <div class="flowchart-point small">
        </div>
        <div class="flowchart-content">
          <div class="card share full-width">
            <div class="card-header clearfix">
              <h5>{{ flowchart.header }}</h5>
            </div>
            <div class="card-description">
              <p>{{ flowchart.content }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  export default {
    name: 'flowchart',
    props: {
      items: Array
    },
    data() {
      return {
        flowcharts: this.items || []
      }
    }
  }
</script>