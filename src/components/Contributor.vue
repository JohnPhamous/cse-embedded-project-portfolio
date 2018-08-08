<template>
    <div class="contributor">
        <img
            :src="contributor.image"
            :alt="contributor.name"
            class="contributor-image"
        >
        <h3 class="contributor-name">
            <a :href="contributor.url" target="_blank">
                {{ contributor.name }}
            </a>
        </h3>
    </div>    
</template>

<script>
export default {
  props: ["contributor"]
};
</script>

<style scoped>
.contributor {
  width: 80px;
  text-align: center;
  margin-right: 25px;
}
.contributor-image {
  width: 50px;
  border-radius: 50%;
  filter: saturate(0.5);
}
.contributor-name {
  font-family: "Work Sans", sans-serif;
  font-weight: 400;
  margin-top: 0px;
  font-size: 0.8em;
}
a {
  color: black;
}
</style>
