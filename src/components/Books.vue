<template>
  <li class="list-group-item list-group-item-action">
    <router-link to="/details">{{ details.name }}</router-link>
  </li>
</template>

<script>
export default {
  props: ["details"],
  name: "Book",
};
</script>