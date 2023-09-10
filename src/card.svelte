<script lang="ts">
    export let name: String;
    export let src: String;
    export let desc: String;
    let active: Boolean = false;
    const toggle = () => active = ! active;
</script>

<div class="flip-box" on:click={toggle}>
    <div class="flip-box-inner" class:flip-it={active}>
        <div class="flip-box-front">
            <div class="card p-3 card-hover flex flex-col w-full h-full gap-4">
                <div class="title flex justify-center">
                    <h2 class="h2">{name}</h2>
                </div>
                <img {src} alt="image de la carte">
            </div>
        </div>
        <div class="flip-box-back">
            <div class="card p-3 card-hover flex flex-col w-full h-full gap-4">
                <div class="title flex justify-center flex-col gap-10">
                    <h2 class="h2">{name}</h2>
                    <p class="h4">Palmares: <br>{desc}</p>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    .flip-box {
        background-color: transparent;
        width: 300px;
        height: 480px;
        /*border: 1px solid #f1f1f1;*/
        perspective: 1000px; /* Remove this if you don't want the 3D effect */
    }

    .flip-box-inner {
        position: relative;
        width: 100%;
        height: 100%;
        text-align: center;
        transition: transform 0.8s;
        transform-style: preserve-3d;
    }

    .flip-it {
        transform: rotateY(180deg);
    }

    .flip-box-front, .flip-box-back {
        position: absolute;
        width: 100%;
        height: 100%;
        -webkit-backface-visibility: hidden; /* Safari */
        backface-visibility: hidden;
    }

    .flip-box-front {
    }

    .flip-box-back {
        transform: rotateY(180deg);
    }
</style>