<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Adaptiveness
        </v-card-title>
        <v-card-text>
          <p>
            The figma design provided had some interesting designs for the mobile screen,
            which were very difficult because it was not just about resizing the component
            on the screen to fit well on a device with small screen.
            It also has different positioning for different components as well as using components
            that were not used on the desktop and tablet screeen
          <p/>
          <p>
            Adaptive design has it pros and cons as well because even though it offers great flexibility
            It can be pretty difficult to manage as you have to keep on updating 2 different files,
            else the changes on the desktop will not be propagated on mobile
          </p>
          <p>
            - Front end components for each page can be found in <code>./src/components</code> directory <br />
            - The mobile page for the front end components are inside <code>./src/components/mobile</code> directory <br />
            - Users' dashboard components are inside <code>./src/pages</code> directory <br />
            - The mobile page for the users' dashboard components are inside <code>./src/pages_mobile</code> directory <br />
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
