<template>
  <section
    id="recent-projects"
    class="overflow-hidden"
  >
    <v-row no-gutters>
      <v-col
        class="text-left pa-5 white--text"
        cols="12"
        md="6"
        style="background-color: #1cd5ea;"
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateX(25%)"
        />

        <base-heading>
          Proyectos
        </base-heading>

        <base-text class="mb-5">
          Una muestra de los proyectos que hago
          en mi tiempo libre, para profundizar
          conocimientos en tecnologías Web
        </base-text>
        <v-row>
          <!-- PROYECTO 1 -->
          <v-col
            class="text-center pa-5 white--text"
            md="6"
          >
            <v-card
              class="mx-auto"
              max-width="300"
              color="accent"
            >
              <v-img
                class="white--text align-end"
                height="140px"
                :src="require('@/assets/leaflet.png')"
              >
                <v-card-title>
                  Angular + Google Maps
                </v-card-title>
              </v-img>
              <v-card-subtitle class="pb-0 text-left">
                Uso de la librería leaflet.js para trabajar con mapas de google en Angular.
              </v-card-subtitle>

              <v-card-actions>
                <v-btn
                  color="orange"
                  text
                  href="https://angular-leaflet-1.web.app/"
                  target="_blank"
                >
                  Demo
                </v-btn>

                <v-btn
                  color="orange"
                  text
                  href="https://github.com/jofredreinosa/angular-leaflet"
                  target="_blank"
                >
                  Código
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <!-- PROYECTO 2 -->
          <v-col
            class="text-center pa-5 white--text"
            md="6"
          >
            <v-card
              color="accent"
              class="mx-auto"
              max-width="300"
            >
              <v-img
                class="white--text align-end"
                height="140px"
                :src="require('@/assets/amchart.png')"
              >
                <v-card-title>
                  Angular + Amcharts V4
                </v-card-title>
              </v-img>
              <v-card-subtitle class="pb-0 text-left">
                Uso de la librería Amcharts V4 para realizar gráficos en Angular.
              </v-card-subtitle>

              <v-card-actions>
                <v-btn
                  color="orange"
                  text
                  href="https://angular-amcharts-v4.web.app/"
                  target="_blank"
                >
                  Demo
                </v-btn>

                <v-btn
                  color="orange"
                  text
                  href="https://github.com/jofredreinosa/angular-amcharts"
                  target="_blank"
                >
                  Código
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-col>

      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/project2.jpeg')"
          height="100%"
        />
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    name: 'RecentProjects',

    data: () => ({
      projects: [
        'project1',
        'project2',
        'project3',
        'project4',
      ],
    }),
  }
</script>
