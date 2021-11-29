<script>
  import { MDCRipple } from "@material/ripple";

  function materialButton(element) {
    const buttonRipple = new MDCRipple(element);
  }
  export let text;

</script>

<button class="mdc-button" use:materialButton on:click>
  <span class="mdc-button__ripple" />
  <span class="mdc-button__label">{text}</span>
</button>
