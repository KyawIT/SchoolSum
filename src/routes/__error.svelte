<script context="module">
    export function load({ error, status }) {
        return {
            props: {
                errMsg: `${error.message}`,
                errStatus: status,
            }
        };
    }
</script>

<script>
    export let errMsg;
    export let errStatus;
</script>

<svelte:head>
    <title>SchoolSum | Error</title>
    <style>
        body{
            background: linear-gradient( rgba(0, 0, 0, 0.5) 100%, rgba(0, 0, 0, 0.5)100%), url("../../../static/amsterdamLandscape.jpg");
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;
            background-attachment: fixed;
        }
    </style>
</svelte:head>

<div class="err container">
    <div class="position-absolute top-50 start-50 translate-middle">

        <h1 class="text-center text-white text-uppercase">{errMsg}</h1>
        <p class="text-center text-white text-uppercase fs-2">This Site is not available yet.</p>
        <p class="text-center text-white text-uppercase fs-2">Status: {errStatus}</p>
        <div class="text-center">
            <a href="/"><button class="btn btn-primary btn-lg">Go Home</button></a>
        </div>
    </div>
</div>

<style>
    .err{
        height: 80vh;
    }
    .title-err{
    }
</style>
