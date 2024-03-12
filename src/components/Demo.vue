<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="logo"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3 white--text">
          AWS Code Series로 나만의 자동화 구성하기 🌟
        </h1>

          <h4 class="white--text">발표자</h4>

        <p class="subheading font-weight-regular white--text">
          김수민, ACC KHU Captain
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-5 white--text">
          Contact me !
        </h2>

        <v-row justify="center">
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3 white--text"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import logo from '../assets/typo.png'

export default {
  name: 'HelloWorld',

  data: () => ({
    logo,
    whatsNext: [
      {
        text: 'LinkedIn',
        href: 'https://www.linkedin.com/in/Eeap/',
      },
      {
        text: 'GitHub',
        href: 'https://github.com/Eeap',
      },
      {
        text: 'Email',
        href: 'mailto:sumink0903@gmail.com',
      },
    ],
  }),
}
</script>
<style>
  .white--text {
    color: white;
  }
  </style>
