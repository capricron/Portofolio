<template>
    <div class="container">
        <div class="row">
            <div class="col-xl-9 bio">
                <h1><span>Wahyudi</span> Khoeris Salimi</h1>
                <h5>Seorang pelajar yang sangat mencintai dan 
                    antusias terhadap apapun yang berbau teknologi 
                    informasi. Berkeingin mewujudkan dirinya sebagai salah satu penyumbang SDM IT  
                    untuk kemajuan Indonesia dalam keamanan cyber. Dan saat ini sedang dalam masa belajar pengembangan website</h5>
                </div>
            <!-- <div class="col-xl-1 offset-xl-2 sosmed">

            </div> -->
        </div>
        <br>
        <div class="row center">
            <div class="tombol text-center col-xl-4 col-sm-12">
                <a href="mailto:wahyudikhoeris@student.telkom"><h3>Hubungi Saya</h3></a>
            </div>
            <div class="col-xl-3 col-sm-12 sosmed">
                    <a href="https://www.instagram.com/capricron._"><img src="../../assets/sosmed/ig.png" alt="" srcset=""></a>
                    <a href="https://www.facebook.com/ErisCapricron347"><img src="../../assets/sosmed/fb.png" alt="" srcset=""></a>
                    <a href="https://www.linkedin.com/in/wahyudi-khoeris-salimi-15942b198/"><img src="../../assets/sosmed/ld.png" alt="" srcset=""></a>
                    <a href="https://github.com/capricron"><img src="../../assets/sosmed/gh.png" alt="" srcset=""></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Biodata'
}
</script>

<style scoped>
    a{
        color: black;
        text-decoration: none;
    }

    .container{

        margin-bottom: 200px;
    }

    .row{
        margin-top: 50px;
    }
    .bio h1{
        font-size: 50px;
    }
    .bio span{
        color: #f2ca02;
    }
    .bio h5{
        margin-top: 30px;
    }

    .tombol{
        /* margin-top: -40px;
        padding: 5px 20px; */
        padding-top: 5px;
        border-radius: 20px;
        background-color: white;
        width: 300px;
    }

    .sosmed {

        margin-left: 10px;
        /* border-bottom: 2px white solid; */
    }

    .sosmed img{
        margin-left: 20px;
        width: 40px;
    }

    @media (max-width:1000px) {
        .container{
            margin-bottom: 100px;
        }

        .bio h1{
            font-size: 40px;
        }

        .bio span{
            display: block;
        }

        .bio h5{
            font-size: 20px;
        }

        .sosmed{
            padding-left: 10%;
        }

        .sosmed img{
            margin-left: 25px;
            margin-top: 20px;
            width: 40px;
        }

        .tombol{
            margin-left: 10%;
        }


    }
</style>