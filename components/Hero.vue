<template>
  <div class="container">
    <div class="wrapper">
      <h1 class="header">find your fire extinguisher</h1>
      <p class="snippets">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione non sed
        iure officiis. Animi corrupti, fugit soluta voluptas quas impedit
        voluptates. Repudiandae quod atque, hic aspernatur voluptatem vitae
        distinctio iure?
      </p>
      <button>start looking</button>
    </div>
    <img src="../assets/extinguisher.jpg" alt="fire extinguisher" />
  </div>
</template>

<script setup></script>
<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: poppins;
}

.wrapper {
  display: flex;
  flex-direction: column;
  width: 500px;
  align-items: center;
}

.container img {
  width: 300px;
}
</style>
