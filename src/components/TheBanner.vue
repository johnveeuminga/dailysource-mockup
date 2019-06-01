<template>
  <section id='banner' class='banner py-4'>
    <div class="container">
      <h1 class='text-center'>Welcome to the Daily Source</h1>
      <p>
        Our mission is to provide top quality news and information from leading sources across the Internet to educate and inspire you to make the world a better place.
      </p>
      <p>
        Think of us as Google News with human editors and higher ideals. Or as the NPR of the Internet. You will become a better, smarter person by using our website.
      </p>
      <p>
        The Internet has become a jumble of shallow stupidity, noisy nationalism and distracting divisiveness. We help you cut through all that to find the best of what online news has to offer. Learn more about what we offer below.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: 'TheBanner'
}
</script>

<style lang='scss' scoped>
.banner {
  background-color: $gray;
  display: flex;
  height: 550px;
  align-items: center;

  h1 {
    color: $primary;
    font-size: $h2-font-size;
    margin-bottom: 1rem;
    line-height: 1;
  }

  p {
    font-size: 1.625rem;
    max-width: 1100px;
    margin-bottom: 1rem;
    margin-left: auto;
    margin-right: auto;
    text-align: center;

    &:last-child {
      margin-bottom: 0;
    }
  }
}
</style>
