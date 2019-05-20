<template>
  <section class='ways-to-support py-4'>
    <div class="container">
      <h2 class='text-center text-primary'>Ways to support our nonprofit’s work</h2>
      <div class="row">
        <div class="col-md-4 text-center">
          <img src="@/assets/hands-circle.-1.png" alt="">
          <p>We have many virtual volunteer opportunities including news editing, online marketing, research and more.</p>
        </div>
        <div class="col-md-4 text-center">
          <img src="@/assets/heart-donate.b764ea04.png" alt="">
          <p>Help us to provide top quality news that can change the world. We rely on people like you to make it possible.</p>

        </div>
        <div class="col-md-4 text-center">
          <img src="@/assets/social-media.61438aaf.png" alt="">
          <p>Please let your friends know about our news website by following us or posting about us on social media.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'WaysToSupport'
}
</script>

<style lang="scss" scoped>
.ways-to-support {
  background-color: $gray;
  
  h2 {
    margin-bottom: 3rem;
  }

  img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 0.25rem;
    height: 180px;
  }

  p {
    text-align: center;
    font-size: 1.375rem;
  }
}
</style>
