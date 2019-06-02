<template>
  <section id='banner' class='banner py-4'>
    <div class="container">
      <h1 class='text-center'>Welcome to the Daily Source</h1>
      <p>
        Our mission is to provide top quality news and information from leading sources across the Internet to educate and inspire you to make the world a better place. Think of us as Google News with human editors and higher ideals. Or as the NPR of the Internet. 
      </p>
      <p>
        You will become a better, smarter person by using our website. The Internet has become a jumble of noise, selfishness and shallowness. We help you cut through all that to find the best of what the Internet news has to offer. Learn more of what we offer below.
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
  padding-top: 2.625rem !important;
  background-color: $gray;
  height: 450px;
  display: flex;
  align-items: center;

  h1 {
    color: $primary;
    font-size: $h2-font-size;
    margin-bottom: 1.25rem;
    line-height: 1;
  }

  p {
    font-size: 1.5rem;
    max-width: 940px;
    margin-bottom: 1.25rem;
    margin-left: auto;
    margin-right: auto;
    text-align: center;

    &:last-child {
      margin-bottom: 0;
    }
  }
}
</style>
