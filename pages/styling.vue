<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Styling
        </v-card-title>
        <v-card-text>
          <p>
            Although there are some couple of views and components with scoped styles,
            the major styling done is inside <code>./src/css/font-family.css</code> <br />
            The styling is just for the different font sizes needed in the project, from big to small sizes and from thin to thick weight
          <p/>
          <p>
            Bulma CSS Framework was used in styling this project and for things to be eaiser,
            A sass file was created in the sass directory and was used to set style value for
            different properties according to the design system, most especially the primary
            and secondary color code<br />
            The sass file was compiled to generate mystyles.css
          </p>
          <hr />
          <h3>Compile SASS file:</h3>
          <p>
            - Modify mystyles.scss file in the sass folder
            - Delete, rename or backup mystyles.css file in the css folder
            - Open your terminal
            - run <code>npm run sass</code> command to compile and generate mystyles.css file
            in the css folder
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
          </v-btn>git
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>
