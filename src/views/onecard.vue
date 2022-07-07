<template>
  <div>
    <h1>Single card</h1>
    <p>{{ $route.params.id }}</p>
  </div>
</template>

<script>
export default
  props: ["id"],
  data() {
    return {
      id: this.$route.params.id,
      course: null,
    };
  },
  mounted() {
    fetch(" http://localhost:3000/properties/" + this.$route.params.id)
      .then((res) => res.json())
      .then((data) => (this.course = data));
  }
</script>
<style></style>
