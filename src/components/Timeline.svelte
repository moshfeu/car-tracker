<script>
	export const entries = [
    {
      type: 'fuel',
      price: 100
    },
    {
      type: 'treatment',
      price: 200
    },
  ];
</script>

<ul>
{#each entries as item}
  <li>{item.type}</li>
{/each}
</ul>