<template>
  <section class="balance py-4">
    <div class="container">
      <h2 class="text-center text-primary">True balance in multiple ways</h2>
      <p class='balance__subheading'>We choose stories that are balanced about the topics they cover - providing both sides of the story.<br/>More importantly, we address the greatest imbalances of the news media by providing more focus on:</p>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>Good News</h3>
          <img class='d-block mx-auto' src="@/assets/good-news.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other sources:</span> give you 95% bad news with almost no good news. It's really depressing. </p>
          <p>
            <span class="font-weight-bold">DailySource:</span> has news to hearten and inspire you. Further, having enough good news is more accurate. In reality, even when a bad thing occurs in one place, good things occur in others. Thus, we track our ratio of good to bad, and at least 35% of our daily content is good news.
          </p>
        </div>
      </div>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>The bottom half</h3>
          <img class='d-block mx-auto' src="@/assets/the-bottom-half.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other sources:</span> focus almost 100% on the top 20% of people: those making over $4.9 per hour. </p>
          <p>
            <span class="font-weight-bold">DailySource:</span> covers all people equally. So half of our content is about people in the bottom 50%: those making under $1.2 per hour. 14 million die yearly because they earn so little. It’s the biggest problem in the world, but the media ignores it because they're not located here. These people also have it far worse in almost all other key areas including human rights, infrastructure and housing.
          </p>
        </div>
      </div>
      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>Big-picture info</h3>
          <img class='d-block mx-auto' src="@/assets/big-pic-info.png" alt="Good News">
        </div>
        <div class="balance__right">
          <p>
            <span class="font-weight-bold">Other sources:</span>  hit you with isolated events with lots of tiny details that don’t tell you the actual big-picture trend, and often give you a false impression of it.</p>
          <p>
            <span class="font-weight-bold">DailySource:</span> tells you what’s really happening. For example, in a year when crime drops 9%, if you read five stories about single crimes, you’ll wrongly think it’s on the rise. If instead you read one story saying it’s dropped, you get the correct big-picture info with far less effort. The choice is yours: be misinformed with more effort, or be well informed with less effort.
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

  &__subheading {
    font-size: 1.625rem !important;
    max-width: 850px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
  }

  h2 {
    margin-bottom: 2rem;
  }

  h3 {
    font-family: $font-family-base;
    color: $primary;
    text-align: center;
    margin-bottom: 1rem;
    line-height: 1;
  }

  &__section {
    &:not(:last-of-type) {
      margin-bottom: 2rem;
    }
  }

  &__left {
    max-width: 305px;
    flex-grow: 1;
    flex-shrink: 1;
    margin-right: 2rem;
  }

  &__right {
    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 0;
    margin-top: .125rem;
  }
  
  p {
    font-size: 1.375rem;
  }
}
</style>
