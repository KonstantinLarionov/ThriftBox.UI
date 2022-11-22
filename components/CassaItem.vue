<template>
    <div id="wp" class="item-wrapper">
      <div @click="switchmodal_updateCassa()" class="item-update-icon">
                <svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M25.1908 3.1525C25.3426 3.3048 25.4279 3.51108 25.4279 3.72612C25.4279 3.94117 25.3426 4.14745 25.1908 4.29975L23.4959 5.99625L20.2459 2.74625L21.9408 1.04975C22.0931 0.897428 22.2998 0.811859 22.5152 0.811859C22.7307 0.811859 22.9373 0.897428 23.0897 1.04975L25.1908 3.15087V3.1525ZM22.347 7.1435L19.097 3.8935L8.0259 14.9662C7.93647 15.0557 7.86914 15.1647 7.82928 15.2847L6.52115 19.2075C6.49743 19.279 6.49406 19.3557 6.51142 19.429C6.52879 19.5024 6.5662 19.5694 6.61948 19.6227C6.67275 19.676 6.7398 19.7134 6.81312 19.7307C6.88644 19.7481 6.96314 19.7447 7.03465 19.721L10.9574 18.4129C11.0773 18.3735 11.1863 18.3067 11.2759 18.2179L22.347 7.14512V7.1435Z" fill="#F6BD88"/>
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M1.625 21.9375C1.625 22.584 1.88181 23.204 2.33893 23.6611C2.79605 24.1182 3.41603 24.375 4.0625 24.375H21.9375C22.584 24.375 23.204 24.1182 23.6611 23.6611C24.1182 23.204 24.375 22.584 24.375 21.9375V12.1875C24.375 11.972 24.2894 11.7653 24.137 11.613C23.9847 11.4606 23.778 11.375 23.5625 11.375C23.347 11.375 23.1403 11.4606 22.988 11.613C22.8356 11.7653 22.75 11.972 22.75 12.1875V21.9375C22.75 22.153 22.6644 22.3597 22.512 22.512C22.3597 22.6644 22.153 22.75 21.9375 22.75H4.0625C3.84701 22.75 3.64035 22.6644 3.48798 22.512C3.3356 22.3597 3.25 22.153 3.25 21.9375V4.0625C3.25 3.84701 3.3356 3.64035 3.48798 3.48798C3.64035 3.3356 3.84701 3.25 4.0625 3.25H14.625C14.8405 3.25 15.0472 3.1644 15.1995 3.01202C15.3519 2.85965 15.4375 2.65299 15.4375 2.4375C15.4375 2.22201 15.3519 2.01535 15.1995 1.86298C15.0472 1.7106 14.8405 1.625 14.625 1.625H4.0625C3.41603 1.625 2.79605 1.88181 2.33893 2.33893C1.88181 2.79605 1.625 3.41603 1.625 4.0625V21.9375Z" fill="#F6BD88"/>
                </svg>
            </div>
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
        <div @click=switchmodal_deleteCassa() class="item-deletete-icon">
            <svg width="26" height="26" viewBox="0 0 22 25" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M2.0625 1.625C1.63152 1.625 1.2182 1.7962 0.913451 2.10095C0.608705 2.4057 0.4375 2.81902 0.4375 3.25V4.875C0.4375 5.30598 0.608705 5.7193 0.913451 6.02405C1.2182 6.3288 1.63152 6.5 2.0625 6.5H2.875V21.125C2.875 21.987 3.21741 22.8136 3.8269 23.4231C4.4364 24.0326 5.26305 24.375 6.125 24.375H15.875C16.737 24.375 17.5636 24.0326 18.1731 23.4231C18.7826 22.8136 19.125 21.987 19.125 21.125V6.5H19.9375C20.3685 6.5 20.7818 6.3288 21.0865 6.02405C21.3913 5.7193 21.5625 5.30598 21.5625 4.875V3.25C21.5625 2.81902 21.3913 2.4057 21.0865 2.10095C20.7818 1.7962 20.3685 1.625 19.9375 1.625H14.25C14.25 1.19402 14.0788 0.780698 13.774 0.475951C13.4693 0.171205 13.056 0 12.625 0L9.375 0C8.94402 0 8.5307 0.171205 8.22595 0.475951C7.92121 0.780698 7.75 1.19402 7.75 1.625H2.0625ZM6.9375 8.125C7.15299 8.125 7.35965 8.2106 7.51202 8.36298C7.6644 8.51535 7.75 8.72201 7.75 8.9375V20.3125C7.75 20.528 7.6644 20.7347 7.51202 20.887C7.35965 21.0394 7.15299 21.125 6.9375 21.125C6.72201 21.125 6.51535 21.0394 6.36298 20.887C6.2106 20.7347 6.125 20.528 6.125 20.3125V8.9375C6.125 8.72201 6.2106 8.51535 6.36298 8.36298C6.51535 8.2106 6.72201 8.125 6.9375 8.125ZM11 8.125C11.2155 8.125 11.4222 8.2106 11.5745 8.36298C11.7269 8.51535 11.8125 8.72201 11.8125 8.9375V20.3125C11.8125 20.528 11.7269 20.7347 11.5745 20.887C11.4222 21.0394 11.2155 21.125 11 21.125C10.7845 21.125 10.5778 21.0394 10.4255 20.887C10.2731 20.7347 10.1875 20.528 10.1875 20.3125V8.9375C10.1875 8.72201 10.2731 8.51535 10.4255 8.36298C10.5778 8.2106 10.7845 8.125 11 8.125ZM15.875 8.9375V20.3125C15.875 20.528 15.7894 20.7347 15.637 20.887C15.4847 21.0394 15.278 21.125 15.0625 21.125C14.847 21.125 14.6403 21.0394 14.488 20.887C14.3356 20.7347 14.25 20.528 14.25 20.3125V8.9375C14.25 8.72201 14.3356 8.51535 14.488 8.36298C14.6403 8.2106 14.847 8.125 15.0625 8.125C15.278 8.125 15.4847 8.2106 15.637 8.36298C15.7894 8.51535 15.875 8.72201 15.875 8.9375Z" fill="#F688A7"/>
            </svg>
        </div>
        <div v-if="state === 'edit'" >asd</div>
        <div v-else-if="state === 'standart'" >123123</div>
        <!-- Модальное окно удаления счёта -->
        <ModalWindow name="delete check"
        v-if="isModalDeleteVisible"
        v-click-outside="switchmodal_deleteCassa"
        modal_header_title="Удалить кассу"
        >
        <div class="modal-item-div-text">
            Подтвердите удаление
        </div>
        <div class="modal_bottombuttonsDelete">
            <button @click="switchmodal_deleteCassa" class="modal_cancelbtn">Отмена</button>
            <button @click="deleteCassa()" class="modal_acceptbtn">Удалить</button>
        </div>
        </ModalWindow>

        <!-- Модальное окно обновления кассы -->
        <ModalWindow name="update check"
        v-if="isModalUpdateVisible"
        v-click-outside="switchmodal_updateCassa"
        modal_header_title="Обновить кассу"
        >
        <div class="modal_divName"><input class="modal_inputall" placeholder="Название кассы" type="text" id="item-modal-input-name"></div>
        <div class="modal_updatePictr">
            <div class="modal_chooseImage">
            <input type="image">
            </div>
            <div class="modal_divupdateImgSelect">
                <select class="modal_updateImgSelect">
                <option value="">изображение</option>
                <option value="1">1</option>
                <option value="2">2</option>
                </select> 
            </div>
        </div>
        <div class="modal_bottombuttonsUpdate">
            <button @click="switchmodal_updateCassa" class="modal_cancelbtn">Отмена</button>
            <button @click="updateCassa()" class="modal_acceptbtn">Обновить</button>
        </div>
        </ModalWindow>
    </div>
</template>
<script>
import ModalWindow from '~/components/ModalWindow.vue';
import axios from '@/axios';
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
    data(){
        return{
            isModalUpdateVisible: false,
            isModalDeleteVisible: false,
        }
    },
    components: {ModalWindow},
    mounted(){

    },
    methods: {
        switchmodal_updateCassa(){
          if (this.isModalUpdateVisible===true) {
            this.isModalUpdateVisible=false;            
          } else {
            this.isModalUpdateVisible=true;
          } 
        },
        switchmodal_deleteCassa(){
          if (this.isModalDeleteVisible===true) {
            this.isModalDeleteVisible=false;            
          } else {
            this.isModalDeleteVisible=true;
          }
        },
        updateCassa(){
          const cassaname = document.getElementById('item-modal-input-name').value;
          axios({
            method: 'PUT',
            url: 'cassa/updateCassa',
            data:{
              cassaName: cassaname,
              "id": '08dac976-b262-4209-8416-07511b90bada',
              "balance": {
                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa3",
                "updated": "2022-11-13T05:42:59.113Z",
                "amount": 0,
                "amountUSD": 0,
                "amountEUR": 0,
                "amountCash": 0,
                "amountCard": 0
              },
              "predictBalance": {
                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa3",
                "updated": "2022-11-13T05:42:59.113Z",
                "amount": 0,
                "amountUSD": 0,
                "amountEUR": 0,
                "amountCash": 0,
                "amountCard": 0
              },
              "currencyType": 0,
              "currentAmount": 0
            },
          })
        },
        deleteCassa(){
          axios({
            method: 'DELETE',
            url: 'cassa/deleteCassa',
            data:{
              "id": '08daca00-2a77-4632-875f-8546b828fa64',
            },
          })
        },
    }
}
</script>
<style>
@import "../assets/cassaitem.scss";
@import '../assets/cassalist.scss';
@import "../assets/modalwindow.scss";
</style>
