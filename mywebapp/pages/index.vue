<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Altair626's page
      </h1>
      <h2 class="subtitle">
        なんかやる
      </h2>
      <div class="links">
        <a
          href="https://wiki.altair626.work"
          target="_blank"
          class="button--green"
        >
          Wiki
        </a>
        <a
          href="http://blog.altair626.work"
          target="_blank"
          class="button--enji"
        >
          Blog
        </a>
        <a
          href="https://github.com/Vegctrp"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a><br>
        <a
          href="https://www.youtube.com/channel/UC3lNFeJiTq6L3UWoz4g1e-A"
          target="_blank"
          class="button--udukikoh"
        >
          卯月コウ
        </a>
        <a
          href="https://twitter.com/mya626"
          target="_blank"
          class="button--blue"
        >
          Twitter
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
