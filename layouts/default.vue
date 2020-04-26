<template>
  <div>
    <Header />
    <div class="container">
      <div class="columns is-centered">
        <div class="column is-3">
          <SideMenu />
        </div>
        <div class="column is-8">
          <div class="card">
            <div class="card-content">
              <nuxt />
            </div>
          </div>
        </div>
      </div>
    </div>
    <footer class="footer has-margin-top-30" style="padding: 10px 0;">
      <div class="has-text-centered is-size-7">
        &copy; {{ year }}. rudolphk.co.za. All Rights Reserved. Built with
        Nuxt.js
      </div>
    </footer>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import SideMenu from '~/components/SideMenu.vue'

export default {
  components: {
    Header,
    SideMenu
  },
  data() {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>