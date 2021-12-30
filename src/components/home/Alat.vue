<template>
    <div class="alat text-center">
            <h1 >Alat dan Bahasa</h1>
            <div class="row">
                <div v-for="x in jumlahfile" v-bind:key="x" class="col-lg-2 gb">
                    <img class="foto" :src="gambar(x)" alt="" srcset="">
                </div>
            </div>
    </div>
</template>

<script>
export default {
    name: 'Alat',
    // methods: {
    //     gambar(x){
    //         let hasil = `img/${x}.png`
    //         return hasil
    //     }
    // }
    data: function(){
        return{
                x: 1,
                jumlahfile: 11,
                gambar(x){
                    let hasil = [require(`../../assets/alat/${x}.png`)]
                    return hasil
                },
            }
        }
    }
</script>

<style>
    .alat{
        margin-bottom: 200px;
        margin-top: 200px;
    }

    h1{
        font-size: 50px;
    }

    .foto{
        margin: 10px;
        width: 100px;
    }

    .gb{
        margin-top: 50px;
    }
</style>