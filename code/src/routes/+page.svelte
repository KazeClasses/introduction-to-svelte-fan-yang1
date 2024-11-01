<script>
    import Navbar from '../components/Navbar.svelte';
    import Hello from '../components/Hello.svelte';
    let count = 0;

    function handleClick() {
        count += 1;
    }

    function isAnnoying() {
        return count > 10;
    }
    
</script>

<Hello />

<button on:click={handleClick}>
    Poke me! {count} {count === 1 ? 'time' : 'times'}
</button>

{#if isAnnoying()}
    <p style="color:red;">You are annoying</p>
{/if}

