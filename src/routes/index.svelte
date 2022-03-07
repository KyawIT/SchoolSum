<script>
</script>

<svelte:head>
    <title>SchoolSum | Welcome</title>
    <style>
        body{
            background: linear-gradient( rgba(0, 0, 0, 0.7) 100%, rgba(0, 0, 0, 0.8)100%), url("./amsterdam.jpg");
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;
            background-attachment: fixed;
        }
    </style>
</svelte:head>

<main class="home-page">
    <div class="position-absolute top-50 start-50 translate-middle">
        <h1 class="display-1 text-white text-center title-main">Welcome to SchoolSum</h1>
        <div class="text-white fs-3 text-center my-3">
            <p>This is a personal website made by Kyaw Htet Htun.</p>
            <p>This website serves as a place to share summaries across devices <i class="bi bi-phone"></i>.</p>
            <p>For and request make a pull request on GitHub <i class="bi bi-github"></i>.</p>
        </div>
    </div>
</main>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Libre+Baskerville&display=swap');
    /*font-family: 'Libre Baskerville', serif;*/

    .home-page{
        height: 80vh;
    }

    .title-main{
        font-family: 'Libre Baskerville', serif;
    }
</style>