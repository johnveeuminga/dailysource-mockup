<template>
  <section class="ways-to-get-news py-4">
    <div class="container">
      <h2 class='text-center'>Multiple Ways to Get News From Us</h2>
      <p class='subheading'>We make it easy to regularly get your news from us. Life will distract you so we encourage you to set up one of the following now to ensure you remember to take advantage of what we provide:</p>
      <div class="row">
        <div class="col-md-6 ways-to-get-news__col">
          <div class="ways-to-get-news__img-container">
            <img src="@/assets/daily-email.png" alt="" class='ways-to-get-news__img ways-to-get-news__img--email'>
          </div>
          <h3>Daily Headlines Email</h3>
          <p>We’ll send you all the stories we’ve published in the past 24 hours at whatever hour of the day you want:</p>
          <div class="newsletter-form-container">
            <newsletter-form />
          </div>
        </div>
        <div class="col-md-6 ways-to-get-news__col ways-to-get-news__col--twitter">
          <div class="ways-to-get-news__img-container">
            <img src="@/assets/twitter.png" alt="" class='ways-to-get-news__img ways-to-get-news__img--twitter'>
          </div>
          <h3>Twitter</h3>
          <p>Follow our Twitter Feeds</p>
          <ul class='twitter-handles'>
            <li>
              <a href="#">@ <span>DailyTopStories</span></a>: Only the top news stories
            </li>
            <li>
              <a href="#">@ <span>DailySourceNews</span></a>: All the news, no opinion pieces
            </li>
            <li>
              <a href="#">@ <span>DailySource</span></a>: All the news and opinion
            </li>
          </ul>
          <p class='facebook-text text-left'>We also post a few stories daily to our Facebook <a href="#">page</a>.</p>
        </div>
        <div class="col-md-6 ways-to-get-news__col">
          <div class="ways-to-get-news__img-container">
            <img src="@/assets/home.png" alt="" class='ways-to-get-news__img ways-to-get-news__img--home'>
          </div>
          <h3>Make us your home page</h3>
          <p>Make DailySource your home page and you’ll have no chance of missing our great stories. You'll be certain to get high quality information and good news every day. To learn how to do this on your browser, click <a href='#'>here.</a></p>
        </div>
        <div class="col-md-6 ways-to-get-news__col">
          <div class="ways-to-get-news__img-container">
            <img src="@/assets/rss.png" alt="" class='ways-to-get-news__img ways-to-get-news__img--rss'>
          </div>
          <h3>RSS Feeds</h3>
          <p>Subscribe to our RSS feeds</p>
          <ul class='rss-list'>
            <li>Top stories</li>
            <li>All items</li>
            <li>The Good News</li>
            <li>The Daily Quote</li>
            <li>Photo of the Day</li>
            <li>Columns/Op-ed</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import NewsletterForm from '@/components/NewsletterForm'

export default {
  name: 'WaysToGetNews',

  components: {
    NewsletterForm,
  },
}
</script>

<style lang="scss" scoped>
.ways-to-get-news {
  padding-bottom: 0 !important;

  h2 {
    color: $primary;
    margin-bottom: 1.25rem;
    line-height: 1;
  }

  a {
    text-decoration: underline;
    color: $blue;
  }

  .subheading {
    font-size: 1.625rem;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
    margin-bottom: 3rem;
  }

  &__img-container {
    height: 60px;
  }

  &__img {
    height: 60px;
    display: block;
    margin-left: auto;
    margin-right: auto;

    &--twitter {
      height: 70px;
      position: relative;
      top: -8px;
    }
  }

  h3 {
    text-align: center;
    color: $primary;
    margin-top: 10px;
  }

  p {
    text-align: center;
    max-width: 560px;
    margin-left: auto;
    margin-right: auto;
    font-size: 1.375rem;
  }

  .newsletter-form-container {
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
  }

  &__col {
    margin-bottom: 1.5rem;
  }

  .rss-list {
    columns: 2;
    max-width: 450px;
    margin-left: auto;
    margin-right: auto;
    
    li {
      position: relative;
      list-style: none;
      display: flex;
      align-items: center;
      font-size: 1.375rem;

      &:before {
        content: '';
        display: inline-block;
        width: 16px;
        height: 16px;
        background-image: url('../assets/icon_rss.png');
        margin-right: .5em;
      }
    }
  }
}

.twitter-handles {
  max-width: 560px;
  margin-left: auto;
  margin-right: auto;
  list-style-type: none;
  padding-left: 0;

  li {
    font-size: 1.375rem;

    &:first-child {
      a {
        color: #F6C448;
      }
    }

    &:nth-child(2) {
      a {
        color: #6334CE;
      }
    }

    &:nth-child(3) {
      a {
        color: #5DCDE3;
      }
    }

    a {
      text-decoration: none !important;
      color: #212529;

      span {
        color: $blue;
      }
    }
  }
}

.facebook-text {
  padding-left: 6px;
  a {
    color: $blue;
    text-decoration: underline;
  }
}
</style>
