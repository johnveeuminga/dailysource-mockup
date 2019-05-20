<template>
  <section id='banner' class='banner py-4'>
    <div class="container">
      <h1 class='text-center'>Welcome to the Daily Source</h1>
      <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. </p>
      <p>Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. </p>
      <p>Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. </p>
      <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. </p>
      <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. In vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis.</p>
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

  h1 {
    color: $primary;
    font-size: $h2-font-size;
    margin-bottom: 1.25rem;
  }

  p {
    font-size: 1.5rem;
    max-width: 1200px;
    margin-bottom: 1.25rem;
    margin-left: auto;
    margin-right: auto;

    &:last-child {
      margin-bottom: 0;
    }
  }
}
</style>
