<script>
  export let character;
  export let modifier;
  export let status;
  export let element;
  export let roll;
</script>

<style>
  div {
    position: relative;
    top: 0;
    left: 0;
  }

  #blank {
    position: absolute;
    top: 0;
    left: 0;
  }

  #modifier {
    position: relative;
    left: 0px;
    top: 0px;
  }
</style>

<div>
  <img id="blank" src="images/blank.jpg" alt="modifier card" />
  <img id="modifier" src={`images/${modifier}.png`} alt="" />
  {#if status}
    <img id="status" src={`images/${status}.png`} alt={status} />
  {/if}
  {#if character}
    <img id="character" src={`images/${character}.png`} alt={character} />
  {/if}
  {#if element}
    <img id="element" src={`images/${element}.png`} alt={element} />
  {/if}
  {#if roll}
    <img id="roll" src={`images/roll.png`} alt={roll} />
  {/if}

</div>
