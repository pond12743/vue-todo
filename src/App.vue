<template>
  <v-app>
    <div>
      
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
    </div>
    <v-app-bar app color="green darken-4" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="data:image/png;base64,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"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn to="/" text>
        <span class="mr-2">Home</span>
      </v-btn>
      <v-btn to="/" text>
        <span class="mr-2">About</span>
      </v-btn>
      <v-btn to="/todo" text>
        <span class="mr-2">Todo</span>
      </v-btn>

    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
  
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
