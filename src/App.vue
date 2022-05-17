<template>
  <div>
    <HeaderComponent/>
    <JumbotronComponent/>
    <MainComponent/>
    <FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import JumbotronComponent from "./components/JumbotronComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";


export default {
  name: 'App',
  components: {
    HeaderComponent,
    JumbotronComponent,
    MainComponent,
    FooterComponent,
  }
}
</script>

<style lang="scss">
@import'./assets/css/general.scss';
@import'./assets/css/utils.scss';
@import'./assets/css/vars.scss';

</style>
