<template>
    <div class="project">
        <div class="text">
            <h1 class="project-title">{{ project.title }}</h1>
            <!-- <p class="subtitle">{{ project.subtitle }}</p> -->
            <p class="description">
                {{ project.description }}
            </p>

            <h2>Contributors</h2>
            <span class="people">
                <contributor
                    v-for="c in project.contributors"
                    :key="c.name"
                    :contributor="c"
                >
                </contributor>
            </span>
            <a :href="project.link" class="project-link" target="_blank">
                {{ project.linkTitle }}
            </a>
        </div>
        <div class="image">
            <img class="project-image" :src="project.image" :alt="project.subtitle">
        </div>
    </div>    
</template>

<script>
import Contributor from "./Contributor";

export default {
  props: ["project"],
  components: {
    Contributor
  }
};
</script>

<style scoped>
.project {
  display: flex;
  margin-bottom: 50px;
}
.project-title {
  margin-top: 0px;
}
h1 {
  font-family: "Roboto", sans-serif;
  margin-bottom: 0px;
}
h2 {
  font-family: "Roboto", sans-serif;
  font-weight: 200;
  color: #3e3e3e;
}
p.subtitle {
  font-family: "Work Sans", sans-serif;
  color: #818181;
  margin-top: 10px;
  text-transform: uppercase;
  letter-spacing: 5px;
  font-size: 1.3em;
  margin-bottom: 0px;
}

p {
  font-family: "Roboto Slab", serif;
}
.people {
  display: flex;
}
.project {
  width: 100%;
}

.text {
  width: 40%;
}

.description {
  width: 80%;
  margin-top: 5px;
  margin-bottom: 25px;
}
.image {
  width: 60%;
}

.project-image {
  width: 100%;
  transition-duration: 0.3s;
}

.project-image:hover {
  transform: translateY(-5px);
  box-shadow: -10px -10px 30px 4px rgba(0, 0, 0, 0.1),
    10px 10px 30px 4px rgba(45, 78, 255, 0.15);
  border-radius: 5px;
}

hr {
  width: 60%;
  margin-left: 0px;
  margin-top: 20px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
}

.project-link {
  font-family: "Work Sans", sans-serif;
  text-transform: uppercase;
  color: #818181;
  text-decoration: none;
  border: 1px solid #818181;
  padding: 10px;
  margin-top: 20px;
  display: inline-block;
}
</style>
