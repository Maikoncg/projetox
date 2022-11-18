<template>
  <b-card id="LocationCard">
    <b-row>
      <b-col cols="12" md="6" class="service-field">
        <b-form-input placeholder="Enter your name"></b-form-input>
      </b-col>
      <b-col cols="12" md="4" class="cep-field">
        <b-form-input placeholder="Seu CEP"></b-form-input>
      </b-col>
      <b-col cols="12" md="6" class="my-location">
        Ativar minha localização
      </b-col>
      <b-col cols="12" md="6" class="find-by-cep">
        Buscar por endereço
      </b-col>
      <b-col cols="12" md="2" class="search-button">
        <b-button block>Buscar</b-button>
      </b-col>
    </b-row>
  </b-card>
</template>

<script>
export default {
  name: 'LocationCard',
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap');
#LocationCard {
  height: auto;
  background: #FFFFFF;
  border-radius: 8px;
  margin: 0 16px;
  padding: 16px;
}
.service-field {
  margin-bottom: 14px;
}
.service-field input, 
.cep-field input {
  background: #EFF6F5;
  border-radius: 12px;
  font-family: 'Open Sans';
  font-size: 16px;
  line-height: 160%;
  color: #142B20;
  height: 58px;
}
.my-location {
  padding-top: 14px;
}
.find-by-cep {
  padding: 12px 0;
}
.my-location,
.find-by-cep {
  font-family: 'Open Sans';
  font-size: 13px;
  font-weight: 400;
  line-height: 17px;
  color: #00B1AC;
  text-align: left;
}
.search-button button {
  background: #00B1AC;
  border-radius: 12px;
  border: 1px solid #00B1AC;
  width: 100%;
  font-family: 'Open Sans';
  font-size: 16px;
  line-height: 26px;
  color: #FFFFFF;
  height: 58px;
}
@media screen and (min-width: 768px) {
  .service-field {
    order: 0;
  }
  .cep-field {
    order: 1;
  }
  .my-location {
    order: 3;
  }
  .find-by-cep {
    text-align: right;
    margin: 12px 0 0 0;
    order: 4;
  }
  .search-button {
    order: 2;
  }
}
</style>