<template>
  <div>
    <div class="icons-container">
      <div
        v-for="item in items"
        :key="item.id"
        class="icon icon-white m-2 d-flex"
      >
        <i
          class="tim-icons"
          :class="item"
        ></i>
        <p style="font-size: x-small; margin-left: 5px; margin-right: 5px">{{ item }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  data() {
    return {
      items: ref([
        'icon-alert-circle-exc',
        'icon-align-center',
        'icon-align-left-2',
        'icon-app',
        'icon-atom',

        'icon-attach-87',
        'icon-badge',
        'icon-bag-16',
        'icon-bank',
        'icon-basket-simple',
        
        'icon-bell-55',
        'icon-bold',
        'icon-book-bookmark',
        'icon-bulb-63',
        'icon-bullet-list-67',

        'icon-bus-front-12',
        'icon-button-pause',
        'icon-button-power',
        'icon-calendar-60',
        'icon-camera-18',

        'icon-caps-small',
        'icon-cart',
        'icon-chart-bar-32',
        'icon-chart-pie-36',
        'icon-chat-33',

        'icon-check-2',
        'icon-cloud-download-93',
        'icon-cloud-upload-94',
        'icon-coins',
        'icon-compass-05',

        'icon-controller',
        'icon-credit-card',
        'icon-delivery-fast',
        'icon-double-left',
        'icon-double-right',

        'icon-email-85',
        'icon-gift-2',
        'icon-globe-2',
        'icon-headphones',
        'icon-heart-2',

        'icon-html5',
        'icon-image-02',
        'icon-istanbul',
        'icon-key-25',
        'icon-laptop',

        'icon-light-3',
        'icon-link-72',
        'icon-lock-circle',
        'icon-map-big',
        'icon-minimal-down',

        'icon-minimal-left',
        'icon-minimal-right',
        'icon-minimal-up',
        'icon-mobile',
        'icon-molecule-40',

        'icon-money-coins',
        'icon-notes',
        'icon-palette',
        'icon-paper',
        'icon-pencil',

        'icon-pin',
        'icon-planet',
        'icon-puzzle-10',
        'icon-satisfied',
        'icon-scissors',

        'icon-send',
        'icon-settings-gear-63',
        'icon-settings',
        'icon-simple-add',
        'icon-simple-delete',

        'icon-simple-remove',
        'icon-single-02',
        'icon-single-copy-04',
        'icon-sound-wave',
        'icon-spaceship',

        'icon-square-pin',
        'icon-support-17',
        'icon-tablet-2',
        'icon-tag',
        'icon-tap-02',

        'icon-tie-bow',
        'icon-time-alarm',
        'icon-trash-simple',
        'icon-triangle-right-17',
        'icon-trophy',

        'icon-tv-2',
        'icon-upload',
        'icon-user-run',
        'icon-vector',
        'icon-video-66',

        'icon-volume-98',
        'icon-wallet-43',
        'icon-watch-time',
        'icon-wifi',
        'icon-world',

        'icon-zoom-split',
        'icon-refresh-01',
        'icon-refresh-02',
        'icon-shape-star',
        'icon-components',
      ]),
    };
  },
};
</script>
<style scoped>
.icons-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(100px, 1fr)); /* Adjust the minimum and maximum width as needed */
  gap: 1rem; /* Adjust the gap between icons as needed */
  justify-content: center; /* Center the grid within its container */
  font-size: 80px;
}
</style>
