<template>
  <div>
    <v-card elevation="15">
      <v-card-title>
        <h1 class="accent--text">
          <v-icon v-if="icon" large class="pb-2 accent--text">{{icon}}</v-icon> {{title}}
        </h1>
      </v-card-title>
      <v-card-text class="body-1">
        <slot></slot>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: false
    }
  }
}
</script>
