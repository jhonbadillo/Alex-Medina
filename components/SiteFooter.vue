<template>
  <footer class="site-footer">
    {{ $siteConfig.siteName }} &copy; {{ new Date().getFullYear() }} - Todos los derechos reservados
    <br />
    Hecho con <span style="color: #e25555;">&#9829;</span> desde Sabana de Torres
  </footer>
</template>

<script>
export default {
  name: 'SiteFooter'
}
</script>

<style scoped>
footer {
  background: #eee;
  padding: 20px 10px;
  text-align: center;
  transition: 0.5s ease all;
}
</style>
