<template>
  <v-container>
    <v-row
      align="center"
      justify="center"
    >
      <v-col
        cols="12"
        sm="12"
      >
        <v-card
          elevation="8"
          class="mt-10"
        >
          <v-window v-model="step">
            <v-window-item :value="1">
              <v-row>
                <v-col
                  cols="12"
                  sm="6"
                >
                  <v-card-text class="mt-12">
                    <h4 class="text-center">
                      Login to your account
                    </h4>
                    <h6 class="text-center grey--text">
                      Log in to your account so you can continue building<br>and editing your onboarding flows
                    </h6>
                    <v-row>
                      <v-col
                        cols="12"
                        sm="10"
                      >
                        <v-text-field
                          label="Email"
                          dense
                          outlined
                          color="green"
                          aria-autocomplete="false"
                          class="mt-16 ml-5"
                        />
                        <v-text-field
                          label="Password"
                          type="password"
                          dense
                          outlined
                          color="green"
                          aria-autocomplete="false"
                          class="mt-6 ml-5"
                        />
                        <v-row>
                          <v-col
                            cols="12"
                            sm="7"
                          >
                            <v-checkbox
                              label="Remember me"
                              class="mt-n1 ml-5"
                              color="green"
                            />
                          </v-col>
                          <v-col
                            cols="12"
                            sm="5"
                          >
                            <span class="caption green--text">Forgot password</span>
                          </v-col>
                        </v-row>
                        <v-btn
                          tile
                          color="green"
                          dark
                          block
                          class="mx-3"
                        >
                          Login
                        </v-btn>
                        <h5 class="grey--text text-center mt-4 mb-3">
                          Or login using
                        </h5>
                        <div class="d-flex justify-space-between align-center mx-10 mb-16">
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="red">
                              fab fa-google
                            </v-icon>
                          </v-btn>
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="blue">
                              fab fa-facebook
                            </v-icon>
                          </v-btn>
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="light-blue lighten-3">
                              fab fa-twitter
                            </v-icon>
                          </v-btn>
                        </div>
                      </v-col>
                    </v-row>
                  </v-card-text>
                </v-col>
                <v-col
                  cols="12"
                  sm="6"
                  class="green rounded-bl-xl"
                >
                  <div style="text-align:center; padding:180px 0;">
                    <v-card-text class="white--text">
                      <h3 class="text-center">
                        Don't have an account yet?
                      </h3>
                      <h6 class="text-center">
                        Let's get you all set up so you can start your first<br> onboarding experience
                      </h6>
                    </v-card-text>
                    <div class="text-center">
                      <v-btn
                        outlined
                        dark
                        tile
                        @click="step++"
                      >
                        Sign up
                      </v-btn>
                    </div>
                  </div>
                </v-col>
              </v-row>
            </v-window-item>
            <v-window-item :value="2">
              <v-row>
                <v-col
                  cols="12"
                  sm="6"
                  class="green rounded-br-xl"
                >
                  <div style="text-align:center; padding:180px 0;">
                    <v-card-text class="white--text">
                      <h3 class="text-center">
                        Already signed up ?
                      </h3>
                      <h6 class="text-center">
                        sign in to your account so you can continue building<br>and editing your onboarding flows
                      </h6>
                    </v-card-text>
                    <div class="text-center">
                      <v-btn
                        outlined
                        dark
                        tile
                        @click="step--"
                      >
                        Login
                      </v-btn>
                    </div>
                  </div>
                </v-col>
                <v-col
                  cols="12"
                  sm="6"
                >
                  <v-card-text class="mt-12">
                    <h4 class="text-center">
                      Sign up for an account
                    </h4>
                    <h6 class="text-center grey--text">
                      Let's get you all set up so you can start your first<br> onboarding experience
                    </h6>
                    <v-row>
                      <v-col
                        cols="12"
                        sm="10"
                      >
                        <v-row
                          align="center"
                          justify="center"
                        >
                          <v-col
                            cols="12"
                            sm="6"
                          >
                            <v-text-field
                              label="First name"
                              dense
                              outlined
                              color="green"
                              aria-autocomplete="false"
                              class="mt-9 ml-5"
                            />
                          </v-col>
                          <v-col
                            cols="12"
                            sm="6"
                          >
                            <v-text-field
                              label="Last name"
                              dense
                              outlined
                              color="green"
                              aria-autocomplete="false"
                              class="mt-9 mr-1"
                            />
                          </v-col>
                        </v-row>
                        <v-text-field
                          label="Email"
                          dense
                          outlined
                          color="green"
                          aria-autocomplete="false"
                          class="mt-5 ml-5"
                        />
                        <v-text-field
                          label="Password"
                          type="password"
                          dense
                          outlined
                          color="green"
                          aria-autocomplete="false"
                          class="mt-6 ml-5"
                        />
                        <v-row>
                          <v-col
                            cols="12"
                            sm="6"
                          >
                            <v-checkbox
                              label="I accept"
                              class="mt-n1 ml-5"
                              color="green"
                            />
                          </v-col>
                          <v-col
                            cols="12"
                            sm="6"
                          >
                            <span class="caption green--text">Terms & conditions</span>
                          </v-col>
                        </v-row>
                        <v-btn
                          tile
                          color="green"
                          dark
                          block
                          class="mx-3"
                        >
                          Sign up
                        </v-btn>
                        <h5 class="grey--text text-center mt-4 mb-3">
                          Or sign up using
                        </h5>
                        <div class="d-flex justify-space-between align-center mx-10 mb-16">
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="red">
                              fab fa-google
                            </v-icon>
                          </v-btn>
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="blue">
                              fab fa-facebook
                            </v-icon>
                          </v-btn>
                          <v-btn
                            depressed
                            outlined
                            color="grey"
                          >
                            <v-icon color="light-blue lighten-3">
                              fab fa-twitter
                            </v-icon>
                          </v-btn>
                        </div>
                      </v-col>
                    </v-row>
                  </v-card-text>
                </v-col>
              </v-row>
            </v-window-item>
          </v-window>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    source: String,
  },
  data: () => ({
    step: 1,
  }),
}
</script>
<style >
.v-application .rounded-bl-xl {
  border-bottom-left-radius: 300px !important;
}
.v-application .rounded-br-xl {
  border-bottom-right-radius: 300px !important;
}
.v-application {
  font-family: 'Roboto' !important;
}
</style>
