<script>
  import Card from "./Card.svelte";

  let modifiers = [
    "Double Damage - Bless",
    "Double Damage",
    "Minus 1",
    "Minus 2",
    "No Damage - Curse",
    "Plus 1",
    "Plus 2",
    "Neutral"
  ];

  let counter = 0;
</script>

<main>
  <div on:click={() => (counter = (counter + 1) % modifiers.length)}>
    <Card modifier={modifiers[counter]} />
  </div>
</main>
