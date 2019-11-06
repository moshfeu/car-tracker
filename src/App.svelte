<script>
  import 'semantic-ui-css/semantic.css';
  import Timeline from './components/Timeline.svelte';
  import BottomBar from './components/BottomBar.svelte';
</script>

<style type="text/scss">
.app {
  padding: 10px;
}
</style>

<div class="app">
  <div class="app-inner">
    <Timeline />
    <BottomBar />
  </div>
</div>
