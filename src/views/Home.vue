<template>
  <div class="home">
    <the-header />
    <the-banner />
    <news-section />
    <balance-section />
    <ways-to-get-news />
    <ways-to-support />
  </div>
</template>

<script>
// @ is an alias to /src
import TheHeader from '@/components/TheHeader'
import TheBanner from '@/components/TheBanner'
import NewsSection from '@/components/NewsSection'
import BalanceSection from '@/components/BalanceSection'
import WaysToGetNews from '@/components/WaysToGetNews'
import WaysToSupport from '@/components/WaysToSupport'

export default {
  name: 'home',
  components: {
    TheHeader,
    TheBanner,
    NewsSection,
    BalanceSection,
    WaysToGetNews,
    WaysToSupport,
  }
}
</script>
