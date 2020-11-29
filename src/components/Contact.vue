<template>
  <div>
    <div class="left">
      <img src="@/assets/address.jpeg" alt="Address Icon" class="icon" />
      150 Union Avenue Brooklyn, N.Y. 11206
    </div>
    <div class="left">
      <img src="@/assets/email.webp" alt="Email Icon" class="icon" />
      arturo.alicea@outlook.com
    </div>
    <div class="left">
      <img src="@/assets/phone.png" alt="Phone Icon" class="icon" />
      787-376-2563
      <a
        href="https://www.linkedin.com/in/arturo-alicea-a97a2615b/"
        target="_blank"
        rel="noopener noreferrer"
      >
        <img src="@/assets/linkedin.png" alt="LinkedIn Icon" class="linkedin" />
      </a>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Contact extends Vue {}
</script>

<style scoped>
.icon {
  height: auto;
  width: 5%;
  margin: 0 4px -4px 0;
}

.linkedin {
  height: auto;
  width: 22%;
  float: right;
}

.left {
  text-align: left;
  margin-top: 10px;
}

div {
  font-size: 1.2vw;
}
</style>
