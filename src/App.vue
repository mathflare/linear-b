<template>
  <Navbar brand="MathFlare - Latin to Linear B" />
  <div class="container">
    <h1>
      Translate <span style="color: hsl(162, 100%, 32%)">Latin</span> to
      <span style="color: hsl(202, 100%, 35%)">Linear B</span>
    </h1>
    <hr />
    <Translator />
    <br />
    <p>character mapping table comming soon</p>
    <hr />
    <p class="text-muted user-select-none">
      <a
        href="https://github.com/mathflare/linear-b"
        target="_blank"
        class="text-muted"
        ><i class="bi bi-github"></i> GitHub</a
      >
      |
      <a href="https://twitter.com/mathflare" target="_blank" class="text-muted"
        ><i class="bi bi-twitter"></i> Twitter</a
      >
      |
      <a
        href="https://www.instagram.com/mathflare"
        target="_blank"
        class="text-muted"
        ><i class="bi bi-instagram"></i> Instagram</a
      >
    </p>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Translator from "./components/Translator.vue";
//import CharTable from "./components/CharTable.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Translator,
  },
};
</script>
