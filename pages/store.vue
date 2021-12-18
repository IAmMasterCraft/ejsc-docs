<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <v-card>
        <v-card-title class="headline">
          Frontend Store
        </v-card-title>
        <v-card-text>
          <p>
            - This is used to manage data that needs to be persisted <br />
            - This is done with the help of VueX <br />
            - The store handler can be found in <code>./src/store</code> <br />
            - There are getters and mutations for updating and modifying store records
          <p/>
          <hr />
          <h3>Persisted data include:</h3>
          <p>
            <code>
              {
                user_token, <br />
                web_token, <br />
                user: { <br />
                  address, <br />
                  date_joined, <br />
                  email, <br />
                  firstname, <br />
                  image_url, <br />
                  last_login, <br />
                  lastname, <br />
                }, <br />
                subscription, <br />
                subscription_status, <br />
                isBurgerOpened <br />
                isLoading <br />
                isToast, <br />
                cartItems <br />
                isApp <br />
                signup: { <br />
                  firstname, <br />
                  lastname, <br />
                  email, <br />
                  mobile, <br />
                  password, <br />
                }, <br />
                settings: { <br />
                  plan: [ <br />
                    { <br />
                      name, <br />
                      amount, <br />
                    }, <br />
                    { <br />
                      name, <br />
                      amount, <br />
                    }, <br />
                    { <br />
                      name, <br />
                      amount, <br />
                    }, <br />
                  ], <br />
                }, <br />
                filters: { <br />
                  q, <br />
                  m, <br />
                  s, <br />
                  t, <br />
                  pg, <br />
                  s_dt, <br />
                  e_dt, <br />
                  principle_, <br />
                  all_, <br />
                  case_, <br />
                } <br />
              } <br />
            </code>
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
