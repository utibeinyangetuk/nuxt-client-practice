<template>
  <div class="container">
    <ul>
      <li>
        <nuxt-link to="/">home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/my-items">my-items</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/products">products</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script setup></script>

<style scoped>
.container {
  background-color: peru;
}

ul {
  display: flex;
  justify-content: space-around;
  padding: 10px;
}

ul li::marker {
  content: "⌛";
  font-size: 20px;
}
</style>
