<script>
    let ecoLink = "/summaries/economic/";
    let informaticLink = "/summaries/informatic/";
</script>

<nav class="navbar navbar-light bg-warning fixed-top position-relative">
    <div class="container-fluid">
        <a class="navbar-brand fs-2" href="/">
            <img src="/logo_white_large.png" class="logo-nav">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
            <div class="offcanvas-header">
                <h5 class="offcanvas-title" id="offcanvasNavbarLabel">Menu</h5>
                <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
            </div>
            <div class="offcanvas-body">
                <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="/">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href={informaticLink + "cabs"}>CABS</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" id="offcanvasNavbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            BOBW
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="offcanvasNavbarDropdown">
                            <li><a class="dropdown-item" href={ecoLink+"bobw/marketing"}>Marketing</a></li>
                            <li><a class="dropdown-item" href={ecoLink+"bobw/materials-management"}>Materialwirtschaft</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</nav>

<slot></slot>

<div class="w-100 bg-warning footer-bottom position-relative">
    <footer class="d-flex flex-wrap justify-content-between align-items-center my-4 mx-2">
        <div class="col-md-4 d-flex align-items-center">
            <span class="fs-5 text-black">© 2021 WtW, AG.</span>
        </div>

        <ul class="nav col-md-4 justify-content-end list-unstyled d-flex">
            <li class="me-4"><a target="_blank" class="text-black" href="https://www.instagram.com/asian.boy_2005/"><i  class="bi bi-instagram icon-size"></i></a></li>
            <li class="me-3"><a target="_blank" class="text-black" href="https://twitter.com/KyawHtetHtun65"><i  class="bi bi-twitter icon-size"></i></a></li>
        </ul>
    </footer>
</div>

<style>

    .footer-bottom{
        position: fixed;
        bottom: 0;
        height: 10vh;
    }

    nav{
        height: 10vh;
    }

    .logo-nav{
        width: 10em;
        filter: invert(100%);
    }

    .icon-size{
        font-size: 2rem;
    }

    @media only screen and (max-width: 350px) {
        .logo-nav{
            width: 8em;
        }

        .icon-size{
            font-size: 1.5rem;
        }
    }
</style>