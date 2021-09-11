<template>
  <nav class="flex-center upercase" id="">
    <a class="logo" href="/Home">
      <h5>
        @madjsmail
      </h5>
    </a>

    <ul class="nav flex-center">
      <li>
        <NuxtLink
          class="links"
          v-bind:class="created ? 'nuxt-link-active' : ''"
          to="/Home"
          >Home</NuxtLink
        >
      </li>
      <li>
        <NuxtLink
          class="links"
          v-bind:class="created ? 'nuxt-link-active' : ''"
          to="/Portfolio"
        >
          portfolio
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          class="links"
          v-bind:class="created ? 'nuxt-link-active' : ''"
          to="/about"
          >About</NuxtLink
        >
      </li>
      <li>
        <NuxtLink
          class="links"
          v-bind:class="created ? 'nuxt-link-active' : ''"
          to="/Contact"
          >Contact</NuxtLink
        >
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      created: null
    };
  },
  created() {
    this.created = true;
  }
};
</script>
<style lang="scss">
.page-enter-active,
.page-leave-active {
  transition: opacity 0.5s;
}
.page-enter,
.page-leave-to {
  opacity: 0;
}

</style>
