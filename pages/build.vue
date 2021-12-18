<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Build and Deploy
        </v-card-title>
        <v-card-text>
          <h3>Building the project</h3>
          <p>
            - open your terminal <br />
            - run <code>npm run build</code> to rebuild the dist files and folders<br />
          <p/>
          <hr />
          <h3>Committing your changes to remote repository</h3>
          <p>
            - open your terminal <br />
            - Perform some git first-time operations like chekout to new branch,
            setting remote url... if you have not done so <br />
            - run the following command: <br />
            <code>git add .</code> <br />
            <code>git commit -m "your commit message"</code> <br />
            <code>git push origin branch_name</code><br />
            PS: <i>It might require some authentication from you</i><br />
          </p>
          <hr />
          <h3>Pulling to server</h3>
          <p>
            - Login to server via SSH client with appropriate configs <br />
            - cd into ejsc-demo directory which is at <code>usr/var/html/ejsc-demo</code>
            - run <code>git pull</code> to pull the remote update to server
            PS: <i>It might require some authentication from you</i><br />
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
