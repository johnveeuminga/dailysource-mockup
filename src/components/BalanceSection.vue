<template>
  <section class="balance py-4">
    <div class="container">
      <h2 class="text-center text-primary">True balance in multiple ways</h2>
      <p class='balance__subheading text-center'>We give you stories that are balanced: providing both sides of the story. More importantly, we fix <br /> the greatest imbalances of the news media by giving you balance in the following key areas:</p>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>Bad News &<br/> Good News</h3>
          <img class='d-block mx-auto' src="@/assets/good-news.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other news media:</span> think it’s only news if it’s bad. They have mostly bad news with a bit of good news.</p>
          <p>
            <span class="font-weight-bold">DailySource:</span> We think it’s important to share the good along with the bad because the news shouldn’t only be depressing. It should also hearten and inspire. Having good news is also far more accurate. Even on days where a terrible event happens in one place, many positive things occur in other places. So, we track the amount of good news on our site, and at least a third of the content must be good news.
          </p>
        </div>
      </div>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>The Top 20% &<br/> The Poorest 50%</h3>
          <img class='d-block mx-auto' src="@/assets/the-bottom-half.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other news media:</span> focus almost entirely on the top 30% of people, those making over $5 per hour.</p>
          <p>
            <span class="font-weight-bold">DailySource:</span> Half of our content is about people in the bottom half: those making under $1.5 an hour. 16 million die yearly because they earn so little: the same number as two Holocausts each year. It’s the biggest problem in the world, but the media ignores it because they're not located here. They also have it far worse with human rights, slavery, democracy, infrastructure, clean water and other key things.
          </p>
        </div>
      </div>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>Small Details &<br/> Big-picture info</h3>
          <img class='d-block mx-auto' src="@/assets/big-pic-info.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other news media:</span> focus on single occurences with lots of useless minutiae that don’t tell you much, and even give you a false impression.</p>
          <p>
            <span class="font-weight-bold">DailySource:</span> We tell you what’s really happening. For example, in a year in which suicide drops 18%, if you read five stories about individual suicides, you’ll wrongly think it’s on the rise. If instead you read one story saying it’s dropped, you get the right info with 80% less time. The choice is yours: be misinformed with more effort, or be well informed with less effort. 
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BalanceSection'
}
</script>

<style lang="scss" scoped>
.balance {
  background-color: $gray;
  padding-bottom: 1.5rem !important;

  &__subheading {
    font-size: 1.625rem !important;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 3rem;
  }

  h2 {
    margin-bottom: 1.25rem;
  }

  h3 {
    font-family: $font-family-base;
    color: $primary;
    margin-bottom: 1rem;
    line-height: 1;
  }

  &__section {
    &:not(:last-of-type) {
      margin-bottom: 2rem;
    }
  }

  &__left {
    max-width: 340px;
    flex-grow: 1;
    flex-shrink: 1;
    margin-right: 2rem;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  &__right {
    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 0;
    margin-top: 1.5rem;
  }
  
  p {
    font-size: 1.375rem;
  }
}
</style>
