<template>
  <q-header class="bg-info">
    <q-toolbar>
      <q-btn flat round size="9px" icon="fas fa-arrow-left" to="/" />
      <q-toolbar-title>
        <div class="text-h4 text-weight-bold q-ml-xl q-py-md">The luxury</div>
      </q-toolbar-title>
    </q-toolbar>
  </q-header>
  <!-- ----------------------- -->
  <q-carousel class="gt-xs" style="height: 100vh" animated v-model="slide">
    <q-carousel-slide :name="1" img-src="~assets/bg-11.jpg">
      <div class="row">
        <div class="col-6 absolute-center">
          <div class="text-h2 text-weight-bold text-warning">
            D I S C O V E R
          </div>
          <div class="text-h2 text-weight-bold" style="letter-spacing: 5px">Luxury Bag</div>
          <div class="text-subtitle1 text-weight-light">
            Lorem ipsum dolor sit amet ipsum dolor <br />
            consectetur adipisicing elit. Non
          </div>
          <q-btn class="q-pl-none text-h6" flat no-caps color="warning" label="Find More" @click="onClick" />
        </div>
        <div class="col-6"></div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="2" img-src="~assets/bg-21.jpg">
      <div class="row q-mt-xl">
        <div class="col-6 q-mt-xl q-pr-xl" align="right">
          <q-img src="~assets/item-2-11.png" style="height: 500px; width: 400px" />
        </div>
        <div class="col-6 q-mt-xl q-pl-xl text-white" style="text-align: left">
          <div class="text-h2 text-grey-7 text-weight-bold q-mt-xl">Beyond</div>
          <div class="text-h1 text-grey-9 text-weight-bold q-my-lg">
            The Luxury
          </div>
          <div class="text-h6 text-grey-7 q-my-lg text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque <br /> velit atque eius temporibus incidunt repudiandae quidem <br />
            assumenda ratione ex reprehenderit
          </div>
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="3" img-src="~assets/bg-31.jpg">
      <div class="row q-mt-xl">
        <div class="col-2"></div>
        <div class="col-6 text-white q-mt-xl">
          <div class="text-h1 text-dark text-weight-bold q-mt-lg" style="letter-spacing: 7px;">
            Purus
          </div>
          <div class="text-h3 text-warning">Sollicitude Amet</div>
          <div class="text-h6 text-dark q-my-lg">
            Lorem ipsum dolor sit amet ipsum dolor
            consectetur adipisicing elit. Non
          </div>
          <br />
          <q-btn mo-caps flat class="text-h6" color="warning" label="Find More" @click="onClick" />
        </div>
        <div class="col-4"></div>
      </div>
    </q-carousel-slide>
  </q-carousel>
  <q-carousel class="lt-sm" style="height: 100vh" animated v-model="slide">
    <q-carousel-slide :name="1" img-src="~assets/bg-11.jpg">
      <div class="row">
        <div class="col-xs-12 q-mt-lg">
          <div class="text-h6 text-weight-bold text-warning">
            D I S C O V E R
          </div>
          <div class="text-h4 text-weight-bold" style="letter-spacing: 5px">Luxury Bag</div>
          <div class="text-subtitle1 text-weight-light">
            Lorem ipsum dolor sit amet ipsum dolor <br />
            consectetur adipisicing elit. Non
          </div>
          <q-btn class="q-pl-none text-h6" flat no-caps color="warning" label="Find More" @click="onClick" />
        </div>
        <!-- <div class="col-6"></div> -->
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="2" img-src="~assets/bg-21.jpg">
      <div class="row q-mt-md">
        <div class="col-xs-12 q-mt-sm" align="center">
          <q-img width="250px" src="~assets/item-2-11.png" />
        </div>
        <div class="col-xs-12 q-pl-md text-white">
          <div class="text-h4 text-grey-7 text-weight-bold ">Beyond</div>
          <div class="text-h3 text-grey-9 text-weight-bold q-my-sm">
            The Luxury
          </div>
          <div class="text-subtitle2 text-grey-7 q-my-sm text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem <br />
            assumenda ratione ex reprehenderit
          </div>
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="3" img-src="~assets/bg-31.jpg">
      <div class="row q-mt-md">
        <div class="col-xs-12 text-white q-mt-sm">
          <div class="text-h4 text-dark text-weight-bold q-mt-md" style="letter-spacing: 7px;">
            Purus
          </div>
          <div class="text-h5 text-warning">Sollicitude Amet</div>
          <div class="text-subtitle2 text-dark text-weight-light">
            Lorem ipsum dolor sit amet ipsum dolor
            consectetur adipisicing elit. Non
          </div>
          <br />
          <q-btn no-caps flat color="warning" label="Find More" @click="onClick" />
        </div>
      </div>
    </q-carousel-slide>
  </q-carousel>
  <!-- ----------------------- -->
  <div class="row text-dark q-px-md q-my-md q-col-gutter-md">
    <div class="col-md-4 col-sm-8 col-xs-12">
      <q-card flat class="my-card">
        <q-img src="~assets/column-service-bag-1.jpg"></q-img>
        <q-card-section>
          <div class="text-h6 text-warning text-weight-bold">
            PHARETRA NULLAM EUISMOD
          </div>
          <div class="text-body1 text-grey-5 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-8 col-xs-12">
      <q-card flat class="my-card">
        <q-img src="~assets/column-service-bag-2.jpg"></q-img>
        <q-card-section>
          <div class="text-h6 text-warning text-weight-bold">
            ORNARE RIDICULUS IPSUM
          </div>
          <div class="text-body1 text-grey-5 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-8 col-xs-12">
      <q-card flat class="my-card">
        <q-img src="~assets/column-service-bag-3.jpg"></q-img>
        <q-card-section>
          <div class="text-h6 text-warning text-weight-bold">
            PORTA AENEAN TRISTIQUE
          </div>
          <div class="text-body1 text-grey-5 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
  <!-- ----------------------- -->
  <q-img class="gt-xs" src="~assets/ambrassador-bg.jpg" style="height: 600px">
    <div class="absolute-center" style="letter-spacing: 3px;">
      <div class="text-h1 text-center text-weight-bold" style="letter-spacing: 2rem">The</div>
      <div class="text-h1 text-center text-weight-bold" style="letter-spacing: 2rem">Luxury</div>
      <div class="text-h1 text-center text-weight-bold" style="letter-spacing: 2rem">Style</div>
    </div>
  </q-img>
  <q-img class="lt-sm" src="~assets/ambrassador-bg.jpg" style="height: 600px">
    <div class="absolute-center" style="letter-spacing: 3px;">
      <div class="text-h4 text-center text-weight-bold" style="letter-spacing: 2rem">The</div>
      <div class="text-h4 text-center text-weight-bold" style="letter-spacing: 2rem">Luxury</div>
      <div class="text-h4 text-center text-weight-bold" style="letter-spacing: 2rem">Style</div>
    </div>
  </q-img>
  <!-- ---------for small slideshow-------------- -->
  <div class="q-pa-md gt-xs">
    <q-carousel v-model="slide" transition-prev="slide-right" transition-next="slide-left" swipeable animated
      control-color="primary" padding infinite height="300px" autoplay class="rounded-borders bg-transparent">
      <q-carousel-slide :name="1" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-xs q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height" src="~assets/photodune-1461540-shoes-m-600x720.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="https://i.pinimg.com/originals/54/39/fc/5439fc9762880c5e0e8e0428b10f9bc8.png" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1931082-ladies-handbag-m-600x720.jpg" />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="2" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-xs q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height" src="https://cdn.wallpapersafari.com/55/64/uaN7Tf.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="https://c1.wallpaperflare.com/preview/521/512/16/high-heels-pumps-red-ladies-shoes.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="https://c0.wallpaperflare.com/preview/591/343/667/5be98e464b40f.jpg  " />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="3" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-xs q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height" src="https://wallpaperaccess.com/full/1076793.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="https://images.pexels.com/photos/904350/pexels-photo-904350.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" />
          <q-img class="rounded-borders col-4 full-height" src="https://wallpaperaccess.com/thumb/1839928.jpg" />
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
  <!-- ----------------------- -->
  <div class="row q-pa-md">
    <div class="col-md-6 col-sm-12 col-xs-12">
      <q-img src="~assets/banner-bag-1.jpg"></q-img>
    </div>
    <div class="col-md-6 col-sm-12 col-xs-12 q-mt-sm">
      <q-img src="~assets/banner-bag-2.jpg"></q-img>
    </div>
  </div>
  <hr>
  <!-- ----------------------- -->
  <div class="q-pa-xl" style="text-align:center">
    <div class="text-h6 q-my-md text-weight-bold">MAGNA PARTURIENT COMMODO</div>
    <div class="text-body1 text-grey-8 q-my-md">Maecenas sed diam eget risus varius blandit sit amet non magna. Nullam
      id dolor.</div>
    <q-btn class="q-my-md">Learn More</q-btn>
  </div>
  <!-- ----------------------- -->
  <q-img class="gt-xs" src="https://wallpaperaccess.com/full/4562987.jpg" style="height:500px">
    <div class="
        text-h1 text-white text-weight-bold
        absolute-center
        bg-transparent
      " style="text-align:center">
      The Luxury </div>
    <div class="text-h6 q-mt-xl bg-transparent
 q-mt-lg absolute-center text-white" style="text-align:center">
      Fashion - High Quality - superior - Elite
    </div>
  </q-img>
  <q-img class="lt-sm" src="https://wallpaperaccess.com/full/4562987.jpg" style="height:500px">
    <div class="absolute-center bg-transparent">
      <div class="text-h5 text-white text-weight-bold bg-transparent">
        The Luxury </div>
      <div class="text-h6 q-mt-sm text-white">
        Fashion - High Quality - superior - Elite
      </div>
    </div>
  </q-img>
  <!-- ----------------------- -->
  <div class="row bg-dark gt-xs">
    <div class="col-6 q-px-xl text-grey-5" style="text-align: center">
      <div class="text-h5 q-my-xl text-grey-4">About Us</div>
      <div class="text-body2">
        Cum sociis natoque penatibus et magnis dis parturient montes, nascetur
        ridiculus mus. Morbi leo risus, porta ac consectetur ac, vestibulum at
        eros.
      </div>
      <div class="text-h3 text-weight-bolder q-mt-xl">The Luxury</div>
    </div>
    <div class="col-6 q-px-xl q-my-md">
      <div class="text-h5 text-grey-4">Recent Comments</div>
      <div class="text-h6 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Classy Men Shoes
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-h6 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Blue Casual Suit
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-h6 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Dark Skirt
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-h6 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Luxury Brown Watch
      </div>
      <div style="border:1px solid grey"></div>
    </div>
  </div>
  <div class="row bg-dark lt-sm">
    <div class="col-xs-12 q-px-xl text-grey-5" style="text-align: center">
      <div class="text-h5 q-my-md text-grey-4">About Us</div>
      <div class="text-body2">
        Cum sociis natoque penatibus et magnis dis parturient montes, nascetur
        ridiculus mus. Morbi leo risus, porta ac consectetur ac, vestibulum at
        eros.
      </div>
      <div class="text-h5 text-weight-bolder q-mt-sm q-mb-lg">The Luxury</div>
    </div>
    <div class="col-xs-12 q-px-md q-my-md">
      <div class="text-h5 text-grey-4 text-center">Recent Comments</div>
      <div class="text-subtitle2 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Classy Men Shoes
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-subtitle2 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Blue Casual Suit
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-subtitle2 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Dark Skirt
      </div>
      <div style="border:1px solid grey"></div>
      <div class="text-subtitle2 q-ma-md text-grey">
        <q-icon name="fas fa-angle-right" /> John Doe on Luxury Brown Watch
      </div>
      <div style="border:1px solid grey"></div>
    </div>
  </div>
  <!-- ----------------------- -->

  <!-- ----------------------- -->
</template>

<script>
import { ref } from "vue";
export default {
  data() {
    return {
      slide: ref(1),
    };
  },
};
</script>
