<template>
    <div class="container">
        <h1 class="text-center">Achievement</h1>
        <br>
        <div class="row">
            <div v-for="x in jumlahfile" v-bind:key="x" class="col-lg-4">
                <div class="container blok text-center">
                    <img class="foto" :src="gambar(x)" alt="" srcset="">
                    <p>{{ket[x]}}
                    <br>
                    <a :href="link(x)" target="_blank" rel="noopener noreferrer">{{web[x]}}</a>
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Porto',
    data: function(){
        return{
                x: 1,
                jumlahfile: 4,
                gambar(x){
                    let hasil = [require(`../../assets/porto/${x}.png`)]
                    return hasil
                },
                ket: [
                    0,
                    'Website profile anggota kelompok',
                    'Bot otomatisasi absen sekolah daring',
                    'Katalog digital tkj 3 2021',
                    'Website Profile Kopi Lasem Elmu'
                ],
                web: [
                    0,
                    'wikwik.epizy.com',
                    'github.com/capricron/Bot-Absen-Sekolah',
                    'katalog-tkj3.rf.gd',
                    'kopi-elmu.herokuapp.com'
                ],
                link(x){
                    let hasil = `http://${this.web[x]}`
                    return hasil
                }
            }
        }
    }
</script>

<style scoped>
    h1{
        color: white;
    }
    .foto{    
        width: 95%;
    }

    .blok p{
        font-size: 25px !important;
    }

    .blok a{
        font-size: 20px;
    }

    .blok{
        height: 350px;
        border-radius: 10px;
        padding-top: 20px;
        padding-bottom: 20px;
        background-color: #C4C4C4;
        margin-bottom: 20px;
    }
</style>