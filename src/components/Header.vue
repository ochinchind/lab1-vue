<template>
  <div class="main-header">
    <div class="main-header-logo">
      <img class="main-header-logo-image" src="../assets/logo.png">
    </div>
    <div class="main-header-buttons">
      <a class="main-header-buttons-button" href="#">
        Home
      </a>
      <a class="main-header-buttons-button" href="#">
        Politics
      </a>
      <a class="main-header-buttons-button" href="#">
        Tech
      </a>
      <a class="main-header-buttons-button" href="#">
        Entertainment
      </a>
      <a class="main-header-buttons-button" href="#">
        Travel
      </a>
      <a class="main-header-buttons-button" href="#">
        Sport
      </a>
      <a class="main-header-buttons-search" href="#">
        <img class="main-header-buttons-search-icon" src="../assets/search.svg">
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-header {
  display: flex;
  justify-content: space-between;
}

.main-header-logo {
  width: 40px;
  height: 40px;
}

.main-header-logo-image {
  width: 100%;
  height: 100%;
}

.main-header-buttons {
  display: flex;
  gap: 4;

}

.main-header-buttons-button {
  padding: 0.5rem 1rem;
  color: black;
  text-decoration: none;
}

.main-header-buttons-button:hover {
  text-decoration: underline;
}

.main-header-buttons-search {
  padding: 0rem 1rem;
  color: black;
  text-decoration: none;
  width: 20px;
  transition: all .2s ease-in-out;
}

.main-header-buttons-search-icon {
  width: 100%;
  height: 100%;
}

.main-header-buttons-search:hover {
  transform: scale(1.3);
}
</style>
