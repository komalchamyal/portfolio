<template>
  <div class="menu">
    <div class="menu-item">
      <div class="menu-text">
        About
      </div>
    </div>
    <div class="menu-item">
      <div class="menu-text">
        Projects
      </div>
    </div>
    <div class="menu-item menu-center">
      <div class="menu-text">
        KOMAL
      </div>
    </div>
    <div class="menu-item">
      <div class="menu-text">
        Resume
      </div>
    </div>
    <div class="menu-item">
      <div class="menu-text">
        Contact
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'Nav-bar',
}
</script>

<style scoped>
.menu {
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.menu-item {
  flex: 1;
  text-align: center;

}

.menu-text {
  cursor: pointer;
  border-bottom: 2px solid orange;
  width: fit-content;
}

.menu-center {
  font-size: 2rem;
}
</style>