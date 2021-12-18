<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Setup and Installation
        </v-card-title>
        <v-card-text>
          <h3>Prerequisites and requirements needed:</h3>
          <p>
            - <a href="https://nodejs.org" target="_blank">NodeJS runtime environment</a> installed and running on your machine<br />
            - Text/Code Editor <br />
            - Terminal/Command Line Interface<br />
            - Reliable internet connection (to setup project locally)
          </p>
          <hr />
          <h3>To setup this project on your local machine:</h3>
          <p>
            - Clone the remote repository<br />
            - Open your terminal/command line interface and 'cd' into the project folder<br />
            - run <code>npm install</code> to install dependencies needed for the project to run<br />
            - run <code>npm run serve</code> to start the local server for the project<br />
            This is going to be on port 8080 by default unless the port is busy or occupied by
            another service/program in such case it will assign it a different port which will
            be visible on the terminal<br />
            - open <code>localhost:8080</code> in your browser to run the project
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
