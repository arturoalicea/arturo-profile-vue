<template>
  <div class="card">
    <img src="@/assets/profile.jpeg" class="profile" />
    <h1>Arturo Alicea</h1>
    <p>Fullstack Software Developer</p>
    <a target="_blank" rel="noopener noreferrer" href="./ArturoAlicea-Resume.pdf">
      <img src="@/assets/resume.png" class="resume" />
    </a>
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import Contact from "@/components/Contact.vue";

export default {
  name: "Home",
  components: {
    Contact
  }
};
</script>

<style scoped>
.card {
  background-color: aliceblue;
  border-radius: 25px;
  margin: 0 auto;
  font-family: "BebasNeue";
  padding: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.profile {
  height: auto;
  width: 35%;
  border-radius: 50%;
}

h1 {
  font-size: 3vw;
  font-weight: bold;
  letter-spacing: 5px;
  line-height: 10px;
}

p {
  font-size: 1.5vw;
}

.resume {
  height: auto;
  width: 12%;
  float: right;
  margin: -20px -20px;
}
</style>
