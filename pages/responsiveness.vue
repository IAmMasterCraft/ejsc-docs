<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Responsiveness
        </v-card-title>
        <v-card-text>
          <p>
            Bulma CSS framework was used to make the web app responsive.<br />
            It has several class utility and components that makes development easy and it is
            highly customizable
          <p/>
          <p>You can check out <a href="https://bulma.io/documentation/" target="_blank">Bulma Documentation here</a></p>
        </v-card-text>
        <v-card-actions v-if="true === false">
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>git
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>
