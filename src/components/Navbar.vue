<template>
  <nav class="navbar navbar-expand bg-dark">
    <div class="container">
      <ul class="nav">
        <img src="../assets/logo.png" alt="" />
        <li>
          <router-link to="/" class="nav-link">Katalog</router-link>
        </li>
        <li>
          <router-link to="/manajemen-buku" class="nav-link"
            >Manajemen Buku</router-link
          >
        </li>
      </ul>
    </div>
  </nav>
</template>
<script>
export default {};
</script>
<style>
img {
  height: 40px;
  width: 30px;
}
</style>
