<script lang="ts">

  import Experience from './lib/Experience.svelte';
  import Feedback from './lib/Feedback.svelte';
  import Tutorial from './lib/Tutorial.svelte';
  import Home from './lib/Home.svelte';

  let starting: boolean = true;
  function begin() : void {
    starting = true;
  }
</script>

<main>
  <!--Home on:click={ begin } class={ starting ? "start" : ""}/-->
  {#if starting}
    <div class="menu">
      <Experience />
      <Tutorial />
      <Feedback />
    </div>
  {/if}
</main>
