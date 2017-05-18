<template>
  <flowchart :items="items"></flowchart>
</template>

<script>
import Flowchart from './components/Flowchart.vue';
import Style from './assets/flowchart.css';

export default {
  name: 'app',
  components: {
    Flowchart
  },
  data() {
    return {
      items: [{
        header: "Deneme",
        content: "Deneme content"
      },
      {
        header: "Deneme",
        content: "Deneme content"
      },
      {
        header: "Deneme",
        content: "Deneme content"
      },
      {
        header: "Deneme",
        content: "Deneme content"
      }]
    }
  }
}
</script>
