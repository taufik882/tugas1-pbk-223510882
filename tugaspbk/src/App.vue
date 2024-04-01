<template>
  <div id="app">
    <div class="kontener">
      <header>
        <HeaderCV />
      </header>
      <BodyCV />
    </div>
  </div>
</template>

<script>
import HeaderCV from './components/HeaderCV.vue';
import BodyCV from './components/BodyCV.vue';

export default {
  name: 'App',
  components: {
    HeaderCV,
    BodyCV,
  }
}
</script>

<style scoped>
.kontener{
    background: #f5f5f5;
    max-width: 800px;
    margin: 60px auto;
    height: 1250px;
    padding: 20px;
    box-shadow: 0 2px 2px rgba(0, 0, 0, 0.3);
}
@media only screen and (min-width: 768px) and (max-width: 991px){
  .kontener{
    width: 95%;
    height: auto;
  }
  h2{
    font-size: 10px;
  }
}
@media screen and (max-width: 600px){
  .bodi{
    flex-direction: column;
  }
  .left, .right{
    flex: none;
    width: 100%;
  }
  .kontener{
    width: 95%;
    height: auto;
  }
  h2{
    font-size: 15px;
  }
}
</style>
