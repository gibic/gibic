<script lang="ts">
    export let items = [];
    export let activeTabValue = 1;

    const handleClick = tabValue => () => (activeTabValue = tabValue);
</script>
<div class="tabbed">
    <nav>
        {#each items as item}
        <a href="/" class={activeTabValue === item.value ? 'active' : ''} on:click|preventDefault={handleClick(item.value)}>
            <span>{item.label}</span>
        </a>
        {/each}
        {#each items as item}
            {#if activeTabValue == item.value}
            <div class="box">
                <svelte:component this={item.component}/>
            </div>
            {/if}
        {/each}
    </nav>
</div>
<style>
nav a {
    color: rgba(255, 255, 255, 0.397);
    font-size: larger;
    margin-right: 1rem;
}

nav a.active {
    color: var(--white);
}
nav span {
    display: inline-flex;
    flex-direction: column;
}
nav a.active span::after {
    content: '';
    display: inline-block;
    width: 25px;
    border-bottom: 5px solid #e34c26;
    height: 1px;
}
</style>
