<script>
    let name = 'world';
</script>

<input bind:value={name} placeholder="Enter your name" />
<h1 class="text-4xl text-center text-blue-500">Hello {name}!</h1>
