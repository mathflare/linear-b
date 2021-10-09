<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">{{ brand }}</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbar"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbar">
        <ul class="navbar-nav me-auto my-2 my-lg-0">
        </ul>
        <form class="d-flex">
          <a href="https://www.mathflare.xyz" target="_blank" class="btn btn-outline-light" type="submit">go to MathFlare.xyz</a>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    brand: {
      type: String,
      default: "Vue.js",
      required: true,
    },
  },
};
</script>