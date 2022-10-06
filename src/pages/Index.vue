<template>
  <q-page>
    <q-img fixed alt="Quasar logo" height="100vh" src="~assets/bg-1.jpg">
      <div class="bg-transparent q-mt-xl absolute-center">
        <div class="text-center gt-xs">
          <div class="text-h3 text-bold">T H E L U X U R Y</div>
          <div class="q-ml-xl q-mt-md text-h5 q-mb-lg">Premium Quasar Theme</div>
        </div>
        <div class="text-center lt-sm">
          <div class="text-h6 text-weight-bold">T H E L U X U R Y</div>
          <div class="q-mt-sm text-subtitle2 q-mb-lg">Premium Quasar Theme</div>
        </div>
        <div class="row">
          <div class="col-md-6 col-sm-12 col-xs-12">
            <q-card dark flat class="my-card q-pa-sm gt-xs bg-transparent" @click="DarkStyle">
              <img src="~assets/hp-1.png">
              <q-card-section>
                <div class="text-h6 text-center">DARKSTYLE</div>
              </q-card-section>
            </q-card>
            <q-card dark flat class="my-card q-pa-sm lt-sm bg-transparent" @click="DarkStyle">
              <q-img width="300px" src="~assets/hp-1.png" />
              <q-card-section>
                <div class="text-h6 text-center">DARKSTYLE</div>
              </q-card-section>
            </q-card>
          </div>
          <div class="col-md-6 col-sm-12 col-xs-12 q-mb-xl">
            <q-card dark flat class="my-card q-pa-sm bg-transparent" @click="LightStyle">
              <img src="~assets/hp-2.png">
              <q-card-section>
                <div class="text-h6 text-center">LightStyle</div>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>
    </q-img>
  </q-page>
</template>
<script>
import { useRouter } from "vue-router";
export default {
  setup() {
    const $router = useRouter();
    function DarkStyle() {
      $router.push("/dark");
    }
     function LightStyle() {
       $router.push("/light");
     }
    return {
      DarkStyle,
       LightStyle,
    };
  },
};
</script>
