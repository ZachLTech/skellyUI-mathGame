<script lang="ts">
    import { fade } from 'svelte/transition';
</script>

<div in:fade class="box">
    <h1>Appears from nowhere</h1>
    <p>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error,
      adipisci nihil iste.
    </p>
</div>

<style>
    .box {
      width: 300px;
      border: 1px solid rgb(221, 221, 221);
      padding: 25px;
      border-radius: 10px;
    }
  </style>