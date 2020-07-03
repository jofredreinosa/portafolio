<template>
  <section
    id="about"
    class="overflow-hidden"
  >
    <v-row
      class="white"
      no-gutters
    >
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/aboutme.png')"
          height="100%"
        />
      </v-col>

      <v-col
        class="pa-5"
        cols="12"
        md="6"
        style="background-color: #D8EBF1; color: black;"
      >
        <base-bubble-1 style="transform: translate(5%, -5%)" />

        <base-heading class="info-text">
          Acerca de mí
        </base-heading>

        <base-text class="mb-5">
          Venezolano, actualmente radicado en Santiago de Chile.
          Proactivo, autodidácta, con facilidades para trabajar en
          equipo, capacidad para aprender y enseñar.
          Actualmente trabajando como programador FrontEnd
          con Angular y Angular Material.
        </base-text>

        <base-subheading class="info-text">
          Habilidades Técnicas
        </base-subheading>

        <base-text class="mb-5">
          Las siguientes son algunas de las tecnologías, lenguajes y/o <br>
          frameworks que manejo y/o estoy aprendiendo.
        </base-text>

        <v-alert
          outlined
          color="info"
        >
          <v-list
            two-line
            color="accent"
            dense
          >
            <template v-for="(item, index) in items">
              <v-subheader
                v-if="item.header"
                :key="item.header"
                v-text="item.header"
              />

              <v-divider
                v-else-if="item.divider"
                :key="index"
                :inset="item.inset"
              />

              <v-list-item
                v-else
                :key="item.title"
              >
                <v-list-item-avatar>
                  <v-img :src="item.avatar" />
                </v-list-item-avatar>

                <v-list-item-content>
                  <v-list-item-title v-html="item.title" />
                  <!-- <v-list-item-subtitle v-html="item.subtitle" /> -->
                </v-list-item-content>
              </v-list-item>
            </template>
          </v-list>
        </v-alert>
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    data: () => ({
      items: [
        { header: 'Frontend' },
        {
          avatar: require('@/assets/htmlcssjs.jpg'),
          title: 'Html, Css, JavaScript, Bootstrap',
          subtitle: '',
        },
        { divider: true, inset: true },
        {
          avatar: require('@/assets/angular.png'),
          title: 'Angular, Angular Material, Angular PrimeNG',
          subtitle: '',
        },
        { divider: true, inset: true },
        {
          avatar: require('@/assets/vue.png'),
          title: 'Vue, Vuetify',
          subtitle: '',
        },
        { header: 'Backend' },
        {
          avatar: require('@/assets/laravelphp.png'),
          title: 'Php, Laravel',
          subtitle: '',
        },
        { divider: true, inset: true },
        {
          avatar: require('@/assets/nodeexpress.png'),
          title: 'NodeJs Express',
          subtitle: "<span class='text--primary'>Britta Holt</span> &mdash; We should eat this: Grate, Squash, Corn, and tomatillo Tacos.",
        },
        { header: 'Bases de Datos' },
        {
          avatar: require('@/assets/sql.png'),
          title: 'SQL',
          subtitle: '',
        },
        { divider: true, inset: true },
        {
          avatar: require('@/assets/bbdd.png'),
          title: 'Oracle, MySql, Postgres, SqlServer, MongoDB',
          subtitle: '',
        },
        { header: 'Control de Versiones' },
        {
          avatar: require('@/assets/git.png'),
          title: 'Git, Github',
          subtitle: '',
        },
        { header: 'Oracle' },
        {
          avatar: require('@/assets/oracle.png'),
          title: 'Oracle Forms, Oracle Reports, PL/Sql',
          subtitle: '',
        },
      ],
    }),
  }
</script>
