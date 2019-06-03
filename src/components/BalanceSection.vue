<template>
  <section class="balance py-4">
    <div class="container">
      <h2 class="text-center text-primary">True balance in multiple ways</h2>
      <div class="balance__subheading">
        <!-- <p>We choose stories that are balanced about the topics they cover - providing both sides of the story. </p>
        <p>More importantly, we address the greatest imbalances of the news media by providing more focus on:</p> -->
        <p>
          We give you stories that are balanced about the topics they cover - providing <br />
          both sides of the story. More importantly, we address the greatest imbalances that the <br />
          news media suffers from by providing balance in these important areas: 
        </p>
      </div>

      <div class="balance__section d-flex">
        <div class="balance__left">
          <h3>Bad news and<br />good news</h3>
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
          <h3>The richest half and<br />the poorest half</h3>
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
          <h3>Isolated events and<br />actual trends</h3>
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
    margin-bottom: 3rem;
    
    p {
      font-size: 1.625rem !important;
      margin-left: auto;
      margin-right: auto;
      text-align: center;

      &:last-of-type {
        margin-bottom: 0;
      }
    }
  }

  h2 {
    margin-bottom: 1.25rem;
  }

  h3 {
    font-family: $font-family-base;
    color: $primary;
    font-size: 32px;
    text-align: center;
    margin-bottom: 1rem;
    line-height: 1;
    width: 100%;
  }

  &__section {
    &:not(:last-of-type) {
      margin-bottom: 2rem;
    }

    &:first-of-type {
      margin-top: 3rem;
    }
  }

  &__left {
    max-width: 305px;
    flex-grow: 1;
    flex-shrink: 1;
    margin-right: 2rem;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  &__right {
    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 0;
    margin-top: .5rem;
  }
  
  p {
    font-size: 1.375rem;
  }
}
</style>
