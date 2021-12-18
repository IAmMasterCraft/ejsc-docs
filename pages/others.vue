<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Other Resources and URLs
        </v-card-title>
        <v-card-text>
          <h3>URLs</h3>
          <p>
            - Staging: <a href="https://app.ejsconline.com" target="_blank">app.ejsconline.com</a>
            - Live: <a href="https://portal.ejsconline.com" target="_blank">portal.ejsconline.com</a>
          <p/>
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
