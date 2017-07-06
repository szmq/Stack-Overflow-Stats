<template>
  <div class="phone-viewport">
    <md-toolbar>
      <h2 class="md-title" style="margin-left: 320px;">Stack Overflow Stats</h2>
    </md-toolbar>

    <md-sidenav class="md-left" ref="leftSidenav">
      <md-toolbar class="md-large">
        <div class="md-toolbar-container">
          <h3 class="md-title">User Panel</h3>
        </div>
      </md-toolbar>
      
      <form novalidate @submit.stop.prevent="submit" class="padding">
        <md-input-container>
          <md-icon>search</md-icon>
          <label>Type user name</label>
          <md-input></md-input>
        </md-input-container>
        <md-button class="md-raised md-accent">Submit</md-button>
      </form>
    </md-sidenav>
  </div>
</template>

<script>
export default {
  methods: {
  }
}
</script>

<style>
.md-sidenav.md-left .md-sidenav-content{
  pointer-events: initial;
  transform: translate3D(0, 0, 0);
  box-shadow: 0 4px 5px 0 rgba(0,0,0,0.14), 0 1px 10px 0 rgba(0,0,0,0.12), 0 2px 4px -1px rgba(0,0,0,0.3);
}
</style>
