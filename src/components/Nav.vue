<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><img src="../assets/logo.png" alt=""></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
                <i class="fas fa-bars"></i>
            </button>
            <div class="collapse navbar-collapse" id="navbarScroll">
                <br>
                <ul class="navbar-nav me-auto my-10 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 200px; margin-bottom:250px">
                    <li class="nav-item">
                        <a><router-link class="nav-link" to="/">Home</router-link> </a>
                    </li>
                    <li class="nav-item">
                        <a><router-link class="nav-link" to="/portofolio">Portofolio</router-link></a>
                    </li>
                    <li class="nav-item">
                        <a><router-link class="nav-link" to="/achievement">Achievement</router-link></a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>

<style scoped>
    .navbar{
        position: relative;
        background-color: black;
    }

    i{
        font-size: 30px;
        color: white;
    }

    a:hover{
        color: #f2ca02 !important;
    }

    a{
        color: white;
    }

    .navbar-nav{
        margin-top: -25px !important;
        margin-right: 25px !important;
        position: absolute;
        right: 0;
        font-size: 30px;
        color: white !important;
    }

    @media (max-width:1000px) {
        .navbar-nav{
            position: absolute;
            margin-top: -25px !important;
            margin-left: 10px !important;
            left: 0;
            font-size: 30px;
            color: white !important;
            width: 100%;
            height: 1005;
        }
        
        ul .navbar-nav{
            background-color: violet !important;
            height: 1000px !important;
            margin-top: 1000px !important;
        }

        .collapse{
            margin-bottom: 150px !important;
        }
    }
</style>