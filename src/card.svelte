<script lang="ts">
    export let name: String;
    export let src: String;
</script>

<div class="card p-4 card-hover flex flex-col w-1/4 gap-4">
    <div class="title flex justify-center">
        <h2 class="h2">{name}</h2>
    </div>
    <img {src} alt="image de la carte">
</div>