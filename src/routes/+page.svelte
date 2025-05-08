<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<h1>WELCOME TO THE HTML WEBSITE</h1>
<script>
    let count = 0;

    function increment() {
        count += 1;
    }

    function handleKeydown(event) {
        if (event.code === 'Space') {
            increment();
        }
    }
</script>

<button
    on:click={increment}
    on:keydown={handleKeydown}
    tabindex="0"
    aria-label="Press to increment"
>
    Press me (or Spacebar)
</button>
<p>Button pressed {count} times.</p>