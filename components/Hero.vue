<template>
  <div class="container">
    <div class="wrapper">
      <h1 class="header">find your fire extinguisher</h1>
      <p class="snippets">
        {{ data1 }}
      </p>
      <button>start looking</button>
    </div>
    <img src="../assets/extinguisher.jpg" alt="fire extinguisher" />
  </div>
</template>

 <script>
import { mapState } from 'vuex'

export default {
  computed: {
    ...mapState(['data1', 'data2'])
  }
}
</script>




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
