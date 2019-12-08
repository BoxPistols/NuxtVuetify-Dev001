<template>
<div>
  <h1>{{ mag }}</h1>
  <p>
    <id:>{{ this.$route.params.id }}</id:>
  </p>
</div>
</template>

<script>
export default {
  data: function() {
    return {
      msg: 'users/_id.vue'
    }
  }
}
</script>
