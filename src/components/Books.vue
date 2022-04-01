<template>
  <li>
    <router-link to="/details">{{ details.name }}</router-link>
  </li>
</template>

<script>
export default {
  props: ["details"],
  name: "Book",
};
</script>