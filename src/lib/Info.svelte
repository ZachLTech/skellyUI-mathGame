<script lang="ts">
    import { fade } from 'svelte/transition';
    import calculator from '$lib/assets/calculator.png';
</script>

<div in:fade class="p-5 flex justify-between items-center w-screen h-full">
    <img src={calculator} width="350" alt="Calctoon">
    <p class="p-9 ml-10">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error,
      adipisci nihil iste.
    </p>
</div>
