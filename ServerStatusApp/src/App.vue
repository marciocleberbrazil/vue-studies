<template>
    <div class="container">
        <app-header></app-header>
        <hr>
        <div class="row">
            <app-servers></app-servers>
            <app-server-details></app-server-details>
        </div>
        <hr>
        <app-footer></app-footer>
    </div>
</template>

<script>
  import Footer from './Footer.vue';
  import Header from './Header.vue';
  import Servers from './Servers.vue';
  import ServerDetails from './ServerDetails.vue';
  export default {
      components: {
          'app-footer': Footer,
          'app-header': Header,
          'app-servers': Servers,
          'app-server-details': ServerDetails
      }
  }
</script>
<style>

</style>
