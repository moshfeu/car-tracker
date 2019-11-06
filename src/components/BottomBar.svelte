<script>
  import Icon from 'fa-svelte'
  import { faPlus } from '@fortawesome/free-solid-svg-icons/faPlus'
</script>

<style type="text/scss">
  .bottom-bar {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    padding: 5px;
  }
</style>

<div class="ui fluid three item menu bottom-bar">
  <button class="ui circular twitter icon button add">
    <Icon class="twitter" icon={faPlus}></Icon>
  </button>
</div>