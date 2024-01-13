<template>
  <v-navigation-drawer>
    <v-list>
      <logo />

      <template
        v-for="(item, index) in items"
        :key="index"
      >
        <template v-if="item.subheader">
          <v-list-subheader>{{ item.subheader }}</v-list-subheader>
        </template>

        <template v-else>
          <v-list-item
            :to="item.to"
            :title="item.title"
            exact
            color="primary"
            variant="elevated"
            elevation="0"
            v-bind="item"
          
          />
        </template>
      </template>
    </v-list>
  </v-navigation-drawer>
</template>

<script lang="ts" setup>
const items = [
  { subheader: 'Future' },
  { title: 'Home', prependIcon: 'mdi-home-variant', to: '/' },
  { title: 'Future', prependIcon: 'mdi-faucet', to: '/future' },
  { title: 'Logout', prependIcon: 'mdi-format-title', to: '/logout' },
  { title: 'Contact', prependIcon: 'mdi-page-layout-footer', to: '/contact' }
]
</script>
