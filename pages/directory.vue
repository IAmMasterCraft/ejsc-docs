<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Directory Structure
        </v-card-title>
        <v-card-text>
          <h3>Folders:</h3>
          <p>
            + dist: This contains compiled assets, folders and files.<br />
            It is always regenerated after every build.
          <p/>
          <p>
            + node_modules: This folder houses all installed dependencies.
          <p/>
          <p>
            + public: This folder contains the static files that will not be compiled along with the code as well as the base index.html file
          <p/>
          <p>
            + src: This folder contains all the Vue source code for the project
          </p>

          <hr />

          <h3>More about <i>src</i> folder:</h3>
          <p>
            + assets: This is where almost all media and graphics assets will be found the rest are in public directory
          </p>
          <p>
            + components: This houses vue code for the frontend part of the website (i.e. the part that does not require authentication)
          </p>
          <p>
            + css: this folder contains css code
          </p>
          <p>
            + fonts: this folder contains the font file for the custom font used in the project
          </p>
          <p>
            + pages: This houses vue code for the users' backend part of the website (i.e. the part that does requires authentication)
          </p>
          <p>
            + pages_mobile: mobile vue code for <i>pages</i> folder
          </p>
          <p>
            + router: this folder houses the path route and site navigation
          </p>
          <p>
            + sass: this folder is for syntactically awesome stylesheet
          </p>
          <p>
            + store: This is for managing Vuex store and different state in the web app
          </p>
          <p>
            + views: This houses vue code for each separate page on the web app
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
