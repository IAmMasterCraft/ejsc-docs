<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Assets and Static Files
        </v-card-title>
        <v-card-text>
          <p>
            All special svg icons, png and graphical content are present in this folder
          <p/>
          <p>The pictures of the entire team members used on the website can be found in the teams folder</p>
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
