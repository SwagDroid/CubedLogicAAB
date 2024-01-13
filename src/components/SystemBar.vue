<template>
  <v-system-bar
    color="#262626"
    height="56"
  >
    <div class="d-flex align-center">
      <v-app-bar-nav-icon
        class="d-inline-block d-md-none"
        @click="emit('click:toggle')"
      />

      <div id="app" >
        <img  height="56"  src="../assets/Pirate_Flag.svg">
    </div>
      <div class="text-body-2 font-weight-black ms-2 d-none d-md-block">
        SwagDroid
      </div>
 
    </div>

    <v-spacer />

    <!-- <v-btn
      append-icon="mdi-open-in-new"
      color="primary"
      href="https://store.vuetifyjs.com/products/nebula-ui-kit/"
      rel="noopener"
      target="_blank"
      text="Buy now"
      variant="flat"
    /> -->
<v-btn text="Home"  
      to="/" 
      color="primary"
      target="Home"
      variant="flat"
      class="ms-6 me-2"
/>

<v-btn text="Quote"  
      to="/Quote" 
      color="primary"
      target="About us"
      variant="flat"
      class="ms-6 me-2"
/>

<v-btn text="Sign Up" 
      color="primary"
      target="Portfolio"
      variant="flat"
      class="ms-6 me-2"
/>

<v-btn text="Login" 
      color="primary"
      target="Services"
      variant="flat"
      class="ms-6 me-2"
/>

  </v-system-bar>
</template>

<script lang="ts" setup>
const emit = defineEmits(['click:toggle'])

</script>