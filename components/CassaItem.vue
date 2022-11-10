<template>
    <div id="wp" class="item-wrapper">
        <div class="item-icon">
            <img style="width: 54px; height: 54px; border-radius: 54px;" src="../assets/imgs/54.png"/>
        </div>
        <div class="item-info">
            <div class="item-info-header">Счет карты {{bankName}}</div>
            <div class="item-info-about">{{numberWeekTransactions}} операций за неделю</div>
            <div class="item-info-decription">Основная валюта {{mainCurrency}}</div>
        </div>
        <div class="item-value">
            <div class="item-info-header">{{mainCurrencyTotal}} Руб.</div>
            <div class="item-info-about">{{secondCurrencyTotal}} Дол.</div>
            <div class="item-info-decription">{{thirdCurrencyTotal}} Евр.</div>
        </div>
        <div v-if="state === 'edit'" >asd</div>
        <div v-else-if="state === 'standart'" >123123</div>
    </div>
</template>
<script>
export default {
    layout: "empty",
    props: {
        state: String,
        bankName: String,
        numberWeekTransactions: String,
        mainCurrency: String,
        mainCurrencyTotal: String,
        secondCurrencyTotal: String,
        thirdCurrencyTotal: String,
    },
    mounted(){

    }
}
</script>
<style>
@import "../assets/cassaitem.scss"
</style>
