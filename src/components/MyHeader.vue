<template>
  <div>
    <div class="header-background">
      <div class="header-container">
        <h1 class="logo">BOOLFLIX</h1>
        <div class="input">
          <div>
            <input v-model="filmName" type="text" name="filmname" id="filmname">
            <button @click="$emit('search', filmName)">cerca film</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      filmName: "";
    }
  }
}

</script>

<style lang="scss" scoped>
// HEADER
.header-background {
  background-color: #0e0e0e;
}

.header-container {
  width: 70%;
  margin: 0 auto;
  height: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

// LOGO
.logo {
  height: 100%;
  width: 100px;
  color: red;
}
</style>
