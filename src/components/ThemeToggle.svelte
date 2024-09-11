<script>
    let isGreen = true;

    function toggleColor() {
        const body = document.body;
        if (isGreen) {
            body.classList.remove('bg-green-600');
            body.classList.add('bg-orange-600');
        } else {
            body.classList.remove('bg-orange-600');
            body.classList.add('bg-green-600');
        }
        isGreen = !isGreen;
    }
</script>

<button on:click={toggleColor} class="bg-white text-black p-2 rounded">
    Toggle Background Color
</button>
