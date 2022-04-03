<template>
    <div class="main">
        <h2>Карта города</h2>
        <yandex-map 
        :coords="coords"
        :zoom="13" 
        >
        <ymap-marker 
        :coords="[43.221683,76.858972]" 
        marker-id="1" 
        :icon="{color: 'green'}"
        balloon-template='
            <div style="display:flex">
                <div><img src="https://voxpopuli.kz/img/inner/123/48/dsc_06453.jpg" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№182 Школа гимназия</h3>
                    <p style="margin:6px 3px 3px 3px">4.5/5 Cyber bullying rate</p>
                    <p style="margin:3px">8 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <ymap-marker 
        :coords="[43.236898,76.833493]"
        marker-id="2"
        :icon="{color: 'orange'}"
                balloon-template='
            <div style="display:flex">
                <div><img src="https://wikicity.kz/fotos_ms/Company_6487_PQNrBp2SW0ncK3uDSspY2N.jpeg" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№132 Школа гимназия</h3>
                    <p style="margin:6px 3px 3px 3px">3.5/5 Cyber bullying rate</p>
                    <p style="margin:3px">3 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <ymap-marker 
        :coords="[43.233561,76.910256]"
        marker-id="3"
        :icon="{color: 'green'}"
                balloon-template='
            <div style="display:flex">
                <div><img src="https://avatars.mds.yandex.net/get-altay/1554359/2a0000016a088fff14926802c6ee96a76ae0/XXL" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№32 Школа гимназия</h3>
                    <p style="margin:6px 3px 3px 3px">4.8/5 Cyber bullying rate</p>
                    <p style="margin:3px">3 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <ymap-marker 
        :coords="[43.265945,76.912402]"
        marker-id="4"
        :icon="{color: 'red'}"
        balloon-template='
            <div style="display:flex">
                <div><img src="https://pandaland.kz/upload_text_photo/1584099379__3dfc6f1207ad3221423dd10a1c34900e.jpg" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№49 Школа гимназия</h3>
                    <p style="margin:6px 3px 3px 3px">1.5/5 Cyber bullying rate</p>
                    <p style="margin:3px">9 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <ymap-marker 
        :coords="[43.246863, 76.916584]"
        marker-id="5"
        :icon="{color: 'yellow'}"
        balloon-template='
            <div style="display:flex">
                <div><img src="https://cdn.nur.kz/images/1120/1dc933e38a7de001.jpeg" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№31 Школа </h3>
                    <p style="margin:6px 3px 3px 3px">3.5/5 Cyber bullying rate</p>
                    <p style="margin:3px">9 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <ymap-marker 
        :coords="[43.255221, 76.958224]"
        marker-id="6"
        :icon="{color: 'green'}"
        balloon-template='
            <div style="display:flex">
                <div><img src="https://7zametki.kz/wp-content/uploads/2021/05/image9-1.jpg" height=130 alt=""></div>
                <div style="padding-left:15px">
                    <h3>№121 Школа </h3>
                    <p style="margin:6px 3px 3px 3px">4.7/5 Cyber bullying rate</p>
                    <p style="margin:3px">14 Reviews</p>
                    <p style="margin:3px">Business hours unknowm</p>
                </div>
            </div>'
        />
        <!-- //43.255221, 76.958224 -->
        </yandex-map>
    </div>
</template>

<script>
    import { yandexMap, ymapMarker } from 'vue-yandex-maps'

    export default {
        data: () => {
            return ({
                coords: [
                43.235775, 
                76.919748
                ],

            })
        },
        components:{
            yandexMap, 
            ymapMarker
        },
    }
</script>

<style scoped>
    .main{
        padding: 40px;
    }
    .ymap-container {
        margin-top: 20px;
        height: 500px;

    }
    .balloon p{
        margin: 0px;
    }
</style>