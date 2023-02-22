<script lang="ts">
    let value = 0

    const incr = (amt: number) => () => {value += amt}
</script>

<span>
    <button class="button" on:click={incr(-1)}>-</button>
    {value}
    <button class="button" on:click={incr(1)}>+</button>
</span>