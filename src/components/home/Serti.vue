<template>
    <div class="container">
        <h1 class="text-center">Achievement</h1>
        <br>
        <div class="row">
            <div v-for="x in jumlahfile" v-bind:key="x" class="col-lg-6">
                <div class="container blok text-center">
                    <img class="foto" :src="gambar(x)" alt="" srcset="">
                    <p>{{ket[x]}}
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Serti',
    data: function(){
        return{
                x: 1,
                jumlahfile: 7,
                gambar(x){
                    let hasil = [require(`../../assets/alat/serti/${x}.png`)]
                    return hasil
                },
                ket: [
                    0,
                    'Menyelesaikan pelajaran dasar-dasar Menyelesaikan pelajaran dasar-dasar javascript dari platformkursus coding yaitu progate',
                    'Menyelesaikan pelajaran dasar-dasar python dari platform kursus coding yaitu dicoding',
                    'Menyelesaikan materi dan praktek cara konfigurasi dan menggunakanazure cloud untuk vps dari platform kursus coding yaitu dicoding',
                    'Melakukan konfigurasi jaringan menggunakan cisco paket tracer seperti routing, switching, dan trouble shoting dengan topologi yang sangat komplek',
                    'Melakukan installasi dan konfigurasi server dengan os debian dan windows server. Serta melakukan troubleshoting pada jaringan client maupun server. Pada tingkat Kota',
                    'Melakukan installasi dan konfigurasi server dengan os debian dan windows server. Serta melakukan troubleshoting pada jaringan client maupun server. Pada tingkat Provinsi',
                    'Melakukan implementasi user interface beserta membuat fungsi dari pemrograman CRUD diawasi oleh LSP Informatika'               
                ]
            }
        }
    }
</script>

<style scoped>
    h1{
        color: white;
    }
    .foto{    
        width: 80%;
    }

    .blok p{
        font-size: 25px !important;
    }

    .blok{
        height: 550px;
        border-radius: 10px;
        padding-top: 20px;
        padding-bottom: 20px;
        background-color: #C4C4C4;
        margin-bottom: 20px;
    }
</style>