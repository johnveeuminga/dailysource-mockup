<template>
  <section class="news py-4">
    <div class="container">
      <h2 class='text-center text-primary'>News about making the world better</h2>
      <p class='news__subheading text-center'>We cover the biggest problems in the world to bring attention to them. We also cover positive things people are doing to help, so people will be encouraged and inspired to do more good.  Some of the topics we cover:</p>
      <div class="row news__row-wrapper">
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/nonprofits.png" alt="">
            <h3 class='text-center'>Nonprofits</h3>
            <p>Nonprofits play a major role in helping people and communities. We report on voluntarism, philanthropy, nonprofit trends, innovative ideas and government policies that affect nonprofits.</p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/democracy.png" alt="">
            <h3 class='text-center'>Democracy</h3>
            <p>We focus less on domestic politics and more on the key aspects of democracies such as free and fair elections, the rule of law, political freedom, an independent judiciary and a healthy, vibrant press. </p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/poverty.png" alt="">
            <h3 class='text-center'>Poverty</h3>
            <p>We focus less on domestic politics and more on the key aspects of democracies such as free and fair elections, the rule of law, political freedom, an independent judiciary and a healthy, vibrant press. </p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/human-rights.png" alt="">
            <h3 class='text-center'>Human Rights</h3>
            <p>Nonprofits play a major role in helping people and communities. We report on voluntarism, philanthropy, nonprofit trends, innovative ideas and government policies that affect nonprofits.</p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/science-and-tech.png" alt="">
            <h3 class='text-center'>Science and Tech</h3>
            <p>We bring you stories of people fighting for freedom of speech, assembly and movement, freedom from torture, slavery and arbitrary arrest, and the rights to a fair trial, asylum and personal security.</p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="news__col">
            <img class='news__img' src="@/assets/environment.png" alt="">
            <h3 class='text-center'>Environment</h3>
            <p>Climate change is slated to bring extreme weather, destruction, the spread of diseases, crop failures, geo-political turmoil and economic loss. The first step in improving the world is making sure it doesn’t drive off a cliff.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'NewsSection',
}
</script>

<style lang="scss" scoped>
.news {
  h2 {
    margin-bottom: 1.25rem;
  }

  &__row-wrapper {
    padding-top: 2.5rem;
  }

  &__subheading {
    margin-bottom: 1.625rem;
    font-size: 1.5rem !important;
    max-width: 830px;
    margin-left: auto;
    margin-right: auto;
  }

  &__img {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  h3 {
    margin-top: 0.75rem;
    color: $primary;
    font-family: $font-family-base;
  }

  p {
    font-size: 1.25rem;
  }
}
</style>
