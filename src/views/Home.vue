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
import Contact from "@/components/Contact.vue";

export default {
  name: "Home",
  components: {
    Contact
  }
};
</script>

<style lang="scss" scoped>
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

  @media (max-width: 900px) {
    width: 70%;
    height: auto;
  }
}

.profile {
  height: auto;
  width: 35%;
  border-radius: 50%;
}

h1 {
  font-size: 42px;
  font-weight: bold;
  letter-spacing: 5px;
  line-height: 5px;

  @media (max-width: 900px) {
    font-size: 36px;
  }

  @media (max-width: 600px) {
    font-size: 32px;
    letter-spacing: 0;
    line-height: 0px;
  }
}

p {
  font-size: 20px;

  @media (max-width: 900px) {
    font-size: 16px;
  }

  @media (max-width: 600px) {
    font-size: 14px;
    letter-spacing: 0;
  }
}

.resume {
  height: auto;
  width: 12%;
  float: right;
  margin-right: -15px;

  @media (max-width: 900px) {
    margin-right: -8px;
  }
}
</style>
