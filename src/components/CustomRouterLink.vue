<template>
  <router-link :key="route.path" :to="route.path">
    <div class="custom-link" >
      {{ route.path }}
    </div>
  </router-link>
</template>

<style scoped>
.custom-link {
  background-color: #4caf50;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  border-radius: 8px;
}

.custom-link:hover {
  background-color: #45a049;
}

.custom-link:active {
  background-color: #3e8e41;
}
</style>


<script>
export default {
  name: "CustomRouterLink",
  props: {
    route: Object,
  },
};
</script>