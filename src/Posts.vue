<template>
  <div>
    <h2>{{ post.title }}</h2>
    <p>{{ post.body }}</p>
    <p>{{ post.userId }}</p>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Posts",
  props: {
    post: {
      type: Object,
      required: true,
    },
  },
});
</script>
