<script>
  import { MDCRipple } from '@material/ripple';
  import { onMount } from 'svelte';

  let btnRef;

  onMount(() => {
    new MDCRipple(btnRef);
  });

  export let text;
</script>

<button class="mdc-button" bind:this={btnRef} on:click>
  <span class="mdc-button__ripple" />
  <span class="mdc-button__label">{text}</span>
</button>
