<script setup>
</script>

<template>
  <div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </nav>
    <router-view v-slot="{ Component }">
      <transition>
        <Component :is="Component" />
      </transition>
    </router-view>
  </div>
</template>

<style>

</style>
