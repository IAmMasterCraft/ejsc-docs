<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-switch 
        v-model="isDark" 
        :append-icon="
          `mdi-${ isDark ? 'weather-night' : 'white-balance-sunny' }`
        "
        @change="$vuetify.theme.dark = isDark"
      >
      </v-switch>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      isDark: true,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Setup & Installation',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Directory Structure',
          to: '/directory'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Assets & Static Files',
          to: '/assets'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Styling',
          to: '/styling'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Responsiveness',
          to: '/responsiveness'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Adaptiveness',
          to: '/adaptiveness'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Routing',
          to: '/routing'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Frontend Store',
          to: '/store'
        },
        {
          icon: 'mdi-chart-bubble',
          title: '3rd Party Plugins',
          to: '/plugins'
        },
        // {
        //   icon: 'mdi-chart-bubble',
        //   title: 'API Calls',
        //   to: '/api'
        // },
        {
          icon: 'mdi-chart-bubble',
          title: 'Other Resources & URLs',
          to: '/others'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Build & Deploy',
          to: '/build'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Glossary',
          to: '/glossary'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'EJSC Documentation'
    }
  },
}
</script>
