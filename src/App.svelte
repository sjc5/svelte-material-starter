<script>
  import MaterialButton from "./MaterialButton.svelte";
</script>

<MaterialButton
  text="first button"
  on:click={() => {
    console.log("you just clicked the first button");
  }}
/>
<MaterialButton
  text="second button"
  on:click={() => {
    console.log("you just clicked the second button");
  }}
/>

<style global lang="scss">
  @use "@material/button/styles";
</style>
