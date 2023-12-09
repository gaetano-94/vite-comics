<script>
export default {
  name: 'Main',
};
</script>

<template>
  <main>
    <span>Content goes here</span>
  </main>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;

main {
  height: 135px;
  background-color: $black;
  width: 100%;
  display: flex;
  align-items: center;

  span {
    margin-left: 50px;
    color: white;
    font-size: 25px;
  }
}
</style>
