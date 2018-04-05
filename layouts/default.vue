<template>
  <div>
    <!-- <ul>
      <li><nuxt-link :to="'/'">Home</nuxt-link></li>
      <li><nuxt-link :to="'/about'">About</nuxt-link></li>
      <li><nuxt-link :to="'/contact'">Contact us</nuxt-link></li>
    </ul> -->
    <ul>
      <li><nuxt-link :to="localePath('index')">{{ $t('home') }}</nuxt-link></li>
      <li><nuxt-link :to="localePath('about')">{{ $t('about') }}</nuxt-link></li>
      <li><nuxt-link :to="localePath('contact-us')">{{ $t('contactUs') }}</nuxt-link></li>
    </ul>
    <nuxt/>
    <ul>
      <li><nuxt-link :to="switchLocalePath('en')">English</nuxt-link></li>
      <li><nuxt-link :to="switchLocalePath('fr')">Français</nuxt-link></li>
    </ul>
  </div>
</template>