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
          height="100vh"
        />
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
            class="mt-n10 mr-10"
          >
            <base-heading>Bienvenidos!</base-heading>
            <base-text>
              Hola, me llamo Jofred Reinosa, soy programador,
              trabajé más de 10 años con herramientas de
              desarrollo Oracle como Designer, Forms, Reports y
              PL/Sql.<br>
              En el año 2018 inicié en la
              programación web, tanto en backend como en frontend y
              en la actualidad trabajo y continúo formándome en esta área.
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
