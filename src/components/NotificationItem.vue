<template>
  <li class="notification-item">
    <time>{{ notification.date }}</time>
    <a v-bind:href="notification.link">{{notification.title}}</a>
  </li>
</template>
<script>

export default {
  name: 'NotificationItem',
  props: ['notification']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .notification-item {
    padding-bottom: 8px;
    margin-bottom: 8px;
    border-bottom: 1px solid #ccc;
  }
</style>
