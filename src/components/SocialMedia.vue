<template>
  <div>
    <v-btn
      v-for="(item, i) in items.slice(0, large ? items.length : 3)"
      :key="i"
      fab
      class="ma-2"
      color="info"
      :small="!large"
      :href="item.href"
      target="_blank"
    >
      <v-icon
        dark
        v-text="item.icon"
      />
    </v-btn>
  </div>
</template>

<script>
  export default {
    props: {
      large: {
        type: Boolean,
        default: false,
      },
    },

    data: () => ({
      items: [
        {
          name: 'Twitter',
          icon: 'mdi-twitter',
          href: 'https://twitter.com/reinosaj',
        },
        {
          name: 'Linkedin',
          icon: 'mdi-linkedin',
          href: 'https://www.linkedin.com/in/jofred-reinosa/',
        },
        {
          name: 'Email',
          icon: 'mdi-email',
          href: 'mailto:reinosaj@gmail.com',
        },
      ],
    }),
  }
</script>
