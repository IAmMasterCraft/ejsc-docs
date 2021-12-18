<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Routing
        </v-card-title>
        <v-card-text>
          <p>
            - Router for managing the path and navigation on the browser is at <code>./src/router/index.js</code>.<br />
            - The route is an array of object including the paths and its metadata<br />
            - The page component is imported, and used in its respective route object<br />
            - The Vue Router is also configured to make some checks before and after a url path
            is resolved to ensure that loader comes up and guest do not access auth page 
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
