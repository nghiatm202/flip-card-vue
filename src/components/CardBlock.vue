<template>
  <div class="card">
    <div class="cardInner">
      <div class="cardFace cardFaceFront">
        <div class="cardContent">Front</div>
      </div>
      <div class="cardFace cardFaceBack">
        <div class="cardContent">Back</div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  display: inline-block;
  margin-right: 1rem;
  margin-bottom: 1rem;

  &Inner {
    width: 100%;
    height: 100%;
    transition: transform 1s;
    transform-style: preserve-3d;
    cursor: pointer;
    position: relative;
  }
}
</style>
