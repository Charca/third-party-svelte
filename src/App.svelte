<script lang="ts">
  import FAB from './components/FAB.svelte'
  import Container from './components/Container.svelte'

  let isOpen = false;

  function toggleContainer() {
    isOpen = !isOpen;
  }
</script>

<div>
  <FAB on:click={toggleContainer} />
  {#if isOpen}
    <Container />
  {/if}
</div>
