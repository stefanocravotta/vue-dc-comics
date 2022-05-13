<template>
  <div>

    <HeaderComponent />

    <MainComponent />

    <IconComponent />

    <FooterComponent />

  </div>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from "./components/HeaderComponent.vue";
import IconComponent from './components/IconComponent.vue';
import MainComponent from "./components/MainComponent.vue";


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    IconComponent
}
}
</script>

<style lang="scss">

@import "./assets/style/vars";
@import "./assets/style/global";
@import "./assets/style/utils";
@import "./assets/style/mixins";

</style>
