<template>
  <div class="container">
    <ul>
      <li>home</li>
      <li>about</li>
      <li>products</li>
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
  content: "😱";
 font-size: 20px;
}
</style>
