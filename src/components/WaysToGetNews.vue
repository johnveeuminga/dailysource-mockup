<template>
  <section class="ways-to-get-news py-4">
    <div class="container">
      <h2 class='text-center'>Multiple Ways to Get News From Us</h2>
      <p class='subheading'>We make it easy to regularly get your news from us. Life will distract you so we encourage you to set up one of the following now to ensure you remember to take advantage of what we provide:</p>
      <div class="row">
        <div class="col-md-6 ways-to-get-news__col">
          <img src="@/assets/newsletter.png" alt="" class='ways-to-get-news__img'>
          <h3>Daily Headlines Email</h3>
          <p>We’ll send you all the stories we’ve published in the past 24 hours at whatever hour of the day you want:</p>
          <div class="newsletter-form-container">
            <newsletter-form />
          </div>
        </div>
        <div class="col-md-6 ways-to-get-news__col">
          <img src="@/assets/twitter.png" alt="Twitter Icon" class='ways-to-get-news__img ways-to-get-news__img--twitter'>
          <h3>Twitter</h3>
          <p>Follow Our Twitter timelines</p>
          <ul class='twitter-handles list-unstyled'>
            <li>
              <a href="#">@ <span>DailyTopStories</span></a>: Only the top news stories
            </li>
            <li>
              <a href="#">@ <span>DailySourceNews</span></a>: All the news, no opinion pieces
            </li>
            <li>
              <a href="#">@ <span>DailySource</span></a>: All the news and opinion pieces
            </li>
          </ul>
        </div>
        <div class="col-md-6 ways-to-get-news__col">
          <img src="@/assets/home.png" alt="" class='ways-to-get-news__img ways-to-get-news__img ways-to-get-news__img--home-page'>
          <h3>Make us your home page</h3>
          <div class="ways-to-get-news__home-page-content">
            <!-- <p class='is-marginless'>Make the DailySource your home page so that you'll get good news, great stories and top information every day. To learn how to do this on your browser, click here. To find how to add us to your smartphone home screen, click <a href="#">here.</a></p> -->
            <p class='is-marginless'>
              Make the DailySource your home page so you'll get <br />
              great stories, good news and top information every day. <br />
              To find how to do this on your browser, click <a href="#">here.</a>
            </p>
          </div>
        </div>
        <div class="col-md-6 ways-to-get-news__col ways-to-get-news__col--rss">
          <img src="@/assets/rss.png" alt="" class='ways-to-get-news__img ways-to-get-news__img--rss'>
          <h3>RSS Feeds</h3>
          <div class="ways-to-get-news__rss-content">
            <p>Subscribe to our RSS feeds</p>
            <ul class='rss-list'>
              <li>Top stories</li>
              <li>Columns/Op-ed</li>
              <li>Photo of the Day</li>
            </ul>
            <ul class="rss-list">
              <li>All Items</li>
              <li>Good News</li>
              <li>The Daily Quote</li>
            </ul>
          </div>
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
  padding-top: 2.375rem !important;
  padding-bottom: .375rem !important;

  h2 {
    color: $primary;
    margin-bottom: 1.5rem;
  }

  a {
    color: $blue;
  }

  .subheading {
    font-size: 1.5rem;
    max-width: 875px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
    margin-bottom: 3rem;
  }

  &__img {
    height: 80px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    position: relative

    &--twitter {
      position: relative;
      top: 8px;
    }

    &--rss {
      height: 68px;
      top: 6px;
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
    font-size: 20px;
  }

  .newsletter-form-container {
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
  }

  &__col {
    margin-bottom: 1.5rem;

    &--rss {
      p {
        margin-bottom: 0;
      }
    }
  }

  .rss-list {
    display: flex;
    align-items: center;
    max-width: 575px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 0;
    padding-left: 0;
    flex-wrap: wrap;
    justify-content: space-between;

    &:not(:last-of-type) {
      margin-top: .5rem;
    }

    li {
      position: relative;
      list-style: none;
      display: flex;
      align-items: center;
      font-size: 20px;
      flex-grow: 1;
      flex-shrink: 0;
      min-width: 120px;
      flex-basis: 120px;

            
      &:first-of-type {
        max-width: 165px;
      }

      &:nth-of-type(2) {
        max-width: 195px;
      }

      &:nth-of-type(3) {
        max-width: 180px;
      }

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

  .twitter-handles {
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
    list-style-type: none;

    li {
      font-size: 20px;
      margin-bottom: 0.25em;

      a {
        text-decoration: none !important;
        color: $blue;

        span {
          color: $blue;
        }
      }
    }
  }

  &__home-page-content {
    display: flex;
    align-items: center;
    height: 136px;

    p {
      margin-bottom: 0;
    }
  }
}
</style>
