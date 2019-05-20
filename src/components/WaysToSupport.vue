<template>
  <section class='ways-to-support py-4'>
    <div class="container">
      <h2 class='text-center text-primary'>Ways to support our nonprofit’s work</h2>
      <div class="row">
        <div class="col-md-4">
          <img src="@/assets/hands-circle.-1.png" alt="">
          <p>We have many volunteer opportunities including writing, marketing, research, web development and more.</p>
        </div>
        <div class="col-md-4">
          <img src="@/assets/heart-donate.b764ea04.png" alt="">
          <p>We help nonprofits do great things for the world. We rely on donations from kind people like you to make it possible.</p>
        </div>
        <div class="col-md-4">
          <img src="@/assets/social-media.61438aaf.png" alt="">
          <p>Please let people know about our nonprofit on social media by clicking the buttons above to follow or like us.</p>
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
  h2 {
    margin-bottom: 1.5rem;
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
