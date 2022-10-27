<template>
    <div id="wp" class="item-wrapper">
        <div class="item-icon">
            <img style="width: 54px; height: 54px; border-radius: 54px;" src="../assets/imgs/54.png"/>
        </div>
        <div class="item-info">
            <div class="item-info-header">Счет карты Тинькофф</div>
            <div class="item-info-about">15 операций за неделю</div>
            <div class="item-info-decription">Основная валюта RUB</div>
        </div>
        <div class="item-value">
            <div class="item-info-header">154 000 Руб.</div>
            <div class="item-info-about">2 493,52 Дол.</div>
            <div class="item-info-decription">2 542,93 Евр.</div>
        </div>
        <div v-if="state === 'edit'" >asd</div>
        <div v-else-if="state === 'standart'" >123123</div>
    </div>
</template>
<script>
export default {
    layout: "empty",
    props: {
        state: String
    },
    mounted(){

    }
}
</script>
<style>
@import "../assets/cassaitem.scss"
</style>
