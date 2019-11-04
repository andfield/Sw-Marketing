<template>
  <footer class="footer" :class="{ [`footer-${type}`]: type }">
    <div class="container">
      <nav>
        <ul>
          <li>
            <span>Team Nerdling</span>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Designed by
        Team Nerdlings.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
