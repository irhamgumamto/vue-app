<template>
  <v-footer
    app
    height="40"
  >
  
    <div
      class="text-caption text-disabled"
      style="position: absolute; right: 16px;"
    >
      &copy; 2025 <span class="d-none d-sm-inline-block">Copyright,</span>      
      <a
        class="text-decoration-none on-surface"
        href="https://kalogistics.co.id/about/"
        rel="noopener noreferrer"
        target="_blank"
      >
        PT. Kereta Api Logistik.
      </a>
    </div>
  </v-footer>
</template>

<script setup>
  
</script>

<style scoped lang="sass">
  .social-link :deep(.v-icon)
    color: rgba(var(--v-theme-on-background), var(--v-disabled-opacity))
    text-decoration: none
    transition: .2s ease-in-out

    &:hover
      color: rgba(25, 118, 210, 1)
</style>
