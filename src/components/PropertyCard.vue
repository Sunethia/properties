<template>
  <div class="col-md-3">
    <router-link :to="{ name: 'onecard', params: { id: property.id } }">
      <div class="card m-3" style="width: 18rem">
        <img v-bind:src="property.image" class="img-fluid" />
        <div class="card-body">
          <p class="card-text">{{ property.title }}</p>
          <p class="card-text">{{ property.type }}</p>
          <p class="card-text">{{ property.location }}</p>
          <!-- <p class="card-text">{{ property.size }}</p> -->
          <p class="card-text">{{ property.price }}</p>
        </div>
      </div>
    </router-link>
  </div>
</template>
<script>
export default {
  props: ["property"],
};
</script>
<style scoped>
.cards {
  border: 2px solid black;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  width: 290px;
  height: 370px;
  margin-left: 530px;
}
</style>
