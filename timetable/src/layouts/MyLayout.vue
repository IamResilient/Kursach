<template>
<q-layout view="lHh Lpr lFf">
  <q-layout-header reveal>
    <q-toolbar :inverted="$q.theme === 'ios'">
      <img src="https://www.gsu.by/themes/gsutheme/logo.svg"><h6>Гомельский государственный<br> университет им. Ф. Скориный</h6>
      <q-btn class= "but" label="Панель управления" />
    </q-toolbar>

    <nav-tabs v-if="$q.theme === 'mat'" />
  </q-layout-header>
  <q-page-container>
    <router-view />
  </q-page-container>
</q-layout>
</template>

<script>
import { openURL } from 'quasar'

export default {
  name: 'MyLayout',
  data () {
    return {
      leftDrawerOpen: this.$q.platform.is.desktop
    }
  },
  methods: {
    openURL
  }
}
</script>
