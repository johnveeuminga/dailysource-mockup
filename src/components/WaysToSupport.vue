<template>
  <section class='ways-to-support py-4'>
    <div class="container">
      <h2 class='text-center text-primary'>Ways to support our nonprofit’s work</h2>
      <div class="row">
        <div class="col-md-4 text-center">
          <img src="@/assets/hands-circle.-1.png" alt="">
          <h3>Volunteer</h3>
          <p>We have many virtual volunteer opportunities including news editing, online marketing, research and more.</p>
          <p><a href="#">See details.</a></p>          
        </div>
        <div class="col-md-4 text-center">
          <img src="@/assets/heart-donate.b764ea04.png" alt="">
          <h3>Donate</h3>
          <p>Help us to provide top quality news that can change the world. We rely on people like you to make it possible.</p>
          <p><a href="#">Please donate now.</a></p>          
        </div>
        <div class="col-md-4 text-center">
          <img src="@/assets/social-media.61438aaf.png" alt="">
          <h3>Spread the Word</h3>
          <p>Please let your friends know about our news website by following us or posting about us on social media.</p>
          <p><a href="#">For social media options, click here.</a></p>
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
  padding-bottom: 1.5rem !important;
  background-color: $gray;
  
  h2 {
    margin-bottom: 3rem;
    line-height: 1;
  }

  h3 {
    margin-top: 14px;
    color: $blue;
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

    &:last-child {
      margin-bottom: 0;
    }

    a {
      color: $blue;

      &:hover {
        text-decoration: none;
      }
    }
  }
}
</style>
