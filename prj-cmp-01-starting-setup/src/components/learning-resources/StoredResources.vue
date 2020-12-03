<template>
  <ul>
    <learning-resource-item
      v-for="resource in resources"
      :key="resource.id"
      :title="resource.title"
      :description="resource.description"
      :link="resource.link"
    ></learning-resource-item>
  </ul>
</template>

<script>
import LearningResourceItem from './LearningResourceItem.vue';
export default {
  components: { LearningResourceItem },
  props: ['resources']
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
