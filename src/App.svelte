<script lang="ts">
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Cube from './lib/Cube.svelte'
  import Step from './lib/Step.svelte'
  import Face from './lib/Face.svelte'


</script>

<main>
  <div class="solve">
    <Face />
  </div>
  <div class="solve">
    <Step />
  </div>

</main>

<style>
main
{
  height: 100%;
}
</style>
