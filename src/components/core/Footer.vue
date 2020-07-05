<template>
  <v-footer
    class="justify-center"
  >
    <v-row>
      <v-col
        cols="12"
        class="text-center hidden-sm-and-up"
      >
        <span class="mr-1 blue-grey--text">
          <v-icon>mdi-whatsapp</v-icon>
        </span>
        <span class="mr-7 blue-grey--text">
          +56 9 4010 7086
        </span>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="hidden-xs-only"
      >
        <span class="mr-1 blue-grey--text">
          <v-icon>mdi-whatsapp</v-icon>
        </span>
        <span class="mr-7 blue-grey--text">
          +56 9 4010 7086
        </span>
      </v-col>

      <v-col
        cols="12"
        class="text-center hidden-sm-and-up"
      >
        <span class="mr-1 blue-grey--text">
          <v-icon>mdi-email</v-icon>
        </span>
        <span class="blue-grey--text">
          reinosaj@gmail.com
        </span>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="hidden-xs-only text-right"
      >
        <span class="mr-1 blue-grey--text">
          <v-icon>mdi-email</v-icon>
        </span>
        <span class="blue-grey--text">
          reinosaj@gmail.com
        </span>
      </v-col>

      <!-- <v-col
        class="hidden-sm-and-down"
        :align="'end'"
      >
        <social-media large />
      </v-col>
      <v-col
        class="hidden-md-and-up"
        :align="'center'"
      >
        <social-media large />
      </v-col> -->
    </v-row>
  </v-footer>
</template>

<script>
  export default {
    name: 'CoreFooter',

    components: {
      // SocialMedia: () => import('@/components/SocialMedia'),
    },
  }
</script>
