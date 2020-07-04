<template>
  <v-footer
    height="88"
    class="justify-center"
  >
    <span class="mr-7 blue-grey--text">
      <v-icon class="mr-1">mdi-copyright</v-icon> Jofred Reinosa 2020
    </span>
    <span class="mr-1 blue-grey--text">
      <v-icon>mdi-whatsapp</v-icon>
    </span>
    <span class="mr-7 blue-grey--text">
      +56 9 4010 7086
    </span>
    <span class="mr-1 blue-grey--text">
      <v-icon>mdi-email</v-icon>
    </span>
    <span class="blue-grey--text">
      reinosaj@gmail.com
    </span>
    <v-spacer />
    <social-media large />
  </v-footer>
</template>

<script>
  export default {
    name: 'CoreFooter',

    components: {
      SocialMedia: () => import('@/components/SocialMedia'),
    },
  }
</script>
