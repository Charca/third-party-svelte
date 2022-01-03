<script lang="ts">
  import { fade, fly } from 'svelte/transition';

</script>

<div class="container" transition:fly="{{ y: 20, duration: 250 }}">
  <header></header>
  <main>
    Hello world!
  </main>
</div>

<style>
  .container {
    width: 350px;
    height: 600px;
    border-radius: 6px;
    box-shadow: 0 0 0 1px rgba(0, 0, 0, .05),
                0 5px 30px 0 rgba(0, 0, 0, .15),
                0 3px 3px 0 rgba(0, 0, 0, .05);

    position: fixed;
    bottom: 120px;
    right: 40px;
    display: flex;
    flex-direction: column;
  }

  header {
    background-color: blueviolet;
    border-radius: 6px 6px 0 0;
    height: 50px;
  }

  main {
    display: flex;
    align-items: center;
    justify-content: center;
    flex: 1;
  }
</style>
