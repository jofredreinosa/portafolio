<template>
  <section
    id="welcome"
    class="overflow-hidden"
  >
    <v-row no-gutters>
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/first.jpg')"
          :lazy-src="require('@/assets/first.jpg')"
          class="grey lighten-2"
          :height="'100vh'"
        >
          <template v-slot:placeholder>
            <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
            >
              <v-progress-circular
                indeterminate
                color="black"
              />
            </v-row>
          </template>
        </v-img>
      </v-col>

      <v-col
        class="align-content-space-between layout wrap"
        cols="12"
        md="6"
        :pa-5="$vuetify.breakpoint.smAndDown"
        style="background-color: black;"
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        />

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="10"
            md="6"
            style="color: white;"
          >
            <base-heading class="mt-10">
              Bienvenidos!
            </base-heading>
            <base-text>
              Hola, soy Jofred Reinosa, programador
              con más de 10 años de experiencia en
              desarrollo con Oracle Forms, Reports y
              PL/Sql y en la actualidad, más de 2 años trabajando con
              programación web.
            </base-text>
          </v-col>
        </v-row>

        <!-- <base-bubble-2
          style="transform: rotate(180deg) translate(-200px, -15%)"
        /> -->
      </v-col>
    </v-row>
  </section>
</template>
