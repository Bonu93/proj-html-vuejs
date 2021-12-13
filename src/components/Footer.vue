<template>
  <footer class="h500 d-flex justify-content-center align-items-center">
    <div class="container d-flex justify-content-center align-items-center">
      <div class="row w-75">
        <div class="col-3">
          <ul class="footer-list">
            <li class="title">
              <h4>About</h4>
              <hr class="orange-rule">
            </li>
            <li class="subtitle">
              {{ data.footerAbout.listItem }}
            </li>
          </ul>

        </div>
        <div class="col-3">
            <ul class="footer-list">
            <li class="title">
              <h4>Twitter</h4>
              <hr class="orange-rule">
            </li>
            <li class="subtitle d-flex mb-3"
            v-for="(tweet, i) in data.footerTwitter"
            :key="`tweet-${i}`"
            >
              <div class="icon">
                <i class="fab fa-twitter"></i>
              </div>
              <div>
                {{ tweet.tweet }}
              </div>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <ul class="footer-list">
            <li class="title">
              <h4>Important Links</h4>
              <hr class="orange-rule">
            </li>
            <li class="subtitle"
            v-for="(link, i) in data.footerLinks"
            :key="`link-${i}`"
            >
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <ul class="footer-list">
            <li class="title">
              <h4>Contact Us</h4>
              <hr class="orange-rule">
            </li>
            <li class="subtitle d-flex mb-3"
            v-for="(item, i) in data.footerContacts"
            :key="`item-${i}`"
            >
              <div class="icon">
                <i :class="item.icon"></i>
              </div>
              <div>
                {{ item.text }}
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: {
      data: Object,
    }
}
</script>

<style lang="scss" scoped>
@import '@/styles/globals.scss';


footer {
  background: $black-alt;
  .orange-rule {
    width: 30px;
  }
  ul {
    list-style: none;
    h4 {
      color: $white;
    }
    .subtitle {
      font-size: 12px;
    }
    .icon{
      color: $orange;
      margin-right: 1rem;
    }
    a {
      text-decoration: none;
      color: currentColor;
    }
  }
}
</style>