<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          3rd party plugins
        </v-card-title>
        <v-card-text>
          <p>
            This entails the plugins and dependencies that made the project what it is.
          <p/>
          <hr />
          <h3>Main dependencies</h3>
          <p>
            - axios <br />
            - buefy <br />
            - console-browserify <br />
            - core-js <br />
            - vue <br />
            - vue-axios <br />
            - vue-router <br />
            - vuex <br />
            - vuex-persistedstate <br />
          </p>
          <hr />
          <h3>Dev dependencies</h3>
          <p>
            - vue-cli
            - eslint
            - sass
            - sass-loader
          </p>
          <hr />
          <h3>Other plugins</h3>
          <p>
            - Material Design Icons
            - Fontawesome
            - Paystack
            - Zendesk chat system
          </p>
        </v-card-text>
        <v-card-actions v-if="true === false">
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>
