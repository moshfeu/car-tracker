<script>
  import Icon from 'fa-svelte'
  import { faGasPump } from '@fortawesome/free-solid-svg-icons/faGasPump'
  import { faWrench } from '@fortawesome/free-solid-svg-icons/faWrench'
  import { faMapMarker } from '@fortawesome/free-solid-svg-icons/faMapMarker'
  import { faTint } from '@fortawesome/free-solid-svg-icons/faTint'

	export const entries = [
    {
      type: 'fuel',
      price: 100,
      date: new Date(2019, 8, 23),
      speedometer: 1300,
      location: 'Sonol',
      cost: 150,
      liter: 28
    },
    {
      type: 'treatment',
      price: 200,
      date: new Date(2019, 9, 23),
      speedometer: 1500,
      location: 'Hege',
      cost: 250
    },
  ];

  export const entryMapTypeToIcon = {
    fuel: faGasPump,
    treatment: faWrench
  }
</script>
<style type="text/scss">
  .timeline-icon {
    font-size: 30px;
  }
  .columns {
    display: flex;

    & > div {
      flex: 1;
    }

    & > div:first-child {
      text-align: left;
    }

    & > div:last-child {
      text-align: right;
    }
  }
</style>

<div class="ui feed">
  {#each entries as item}
    <div class="event">
      <div class="label">
        <i class="timeline-icon">
          <Icon icon={entryMapTypeToIcon[item.type]} />
        </i>
      </div>
      <div class="content">
        <div class="summary">
          {item.type}
          <div class="date">
            {item.date.getDate()}/{item.date.getMonth() + 1}/{item.date.getFullYear()}
          </div>
        </div>
        <div class="columns">
          <div>
            <div><Icon icon={faMapMarker} />{item.location}</div>
            {#if item.liter}
            <div><Icon icon={faTint} />{item.liter}ℓ</div>
            {/if}
            {item.speedometer}km
          </div>
          <div>
            {item.cost}
          </div>
        </div>
      </div>
    </div>
  {/each}
</div>