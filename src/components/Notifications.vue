<template>
  <div class="notifications-widget">
    <header>
      <h3 class="title">Notifications</h3>
    </header>
    <ul class="notifications-list">
      <NotificationItem
        v-for="item in list"
        v-bind:notification="item"
        v-bind:key="item.id">
      </NotificationItem>
    </ul>
  </div>
</template>
<script>

import notificationsData from '../data/data.json'
import NotificationItem from './NotificationItem'

export default {
  name: 'Notifications',
  components: {
    NotificationItem
  },
  data () {
    return { list: notificationsData.notifications }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .notifications-widget {
    border-radius: 10px;
    background: #FFF;
    padding: 1em;
    text-align: left;
    width: 300px;
    margin: 0 auto;
  }

  .notifications-list {
    padding: 0;
    margin: 0;
    list-style: none;
  }
</style>
