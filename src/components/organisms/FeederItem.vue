<template lang="pug">
div(class="card")
  div(class="card-block")
    h4(class="card-title")
      router-link(:to="'feeders/' + feeder.id") {{feeder.fullName}}
</template>

<script>
export default {
  name: 'FeederItem',
  props: {
    feeder: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped></style>
