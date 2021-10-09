<template>
  <Navbar brand="Latin to Linear B" />
  <div class="container">
    <h1>
      Translate <span class="underline">Latin</span> to
      <span class="underline">Linear B</span>
    </h1>
    <hr />
    <Translator class="my-5" />
    <br />
    <br />
    <p>character mapping table comming soon</p>
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
