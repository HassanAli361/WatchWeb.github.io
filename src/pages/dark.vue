<template>
  <q-header class="bg-dark">
    <q-toolbar>
      <q-btn flat round size="9px" icon="fas fa-arrow-left" to="/" />
      <q-toolbar-title>
        <div class="text-h4 text-weight-bold q-ml-xl q-py-md">The luxury</div>
      </q-toolbar-title>
    </q-toolbar>
  </q-header>
  <!-- ----------------- -->
  <q-carousel class="gt-xs" style="height: 100vh" animated v-model="slide" navigation autoplay infinite>
    <q-carousel-slide :name="1" img-src="~assets/bg-1.jpg">
      <div class="row q-mt-xl">
        <div class="col-6 q-pt-xl" align="center">
          <q-img class="q-mt-xl" src="~assets/item-1-1.png" style="height: 400px; width: 400px" />
        </div>
        <div class="col-6 q-pt-xl text-white" align="left">
          <div class="text-h3 q-mt-xl">Sky-challanger</div>
          <div class="text-h1 text-weight-bold">Limited Edition</div>
          <div class="text-subtitle1 text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem
            assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
            consequuntur quas nulla.
          </div>
          <br />
          <q-btn class="text-h6 q-pl-none" flat label="Learn More" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="2" img-src="~assets/bg-2.jpg">
      <div class="row q-mt-xl">
        <div class="col-6 q-my-xl text-white" align="right">
          <div class="text-h1 q-mb-md q-mt-xl text-weight-bold">Sport Series</div>
          <div class="text-subtitle1 text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem
            assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
            consequuntur quas nulla.
          </div>
          <br />
          <q-btn class="text-h6 q-pl-none" flat label="Learn More" />
        </div>
        <div class="col-6 q-mt-xl" align="center">
          <q-img class="q-mt-xl q-ml-xl" src="~assets/item-2-2.png" style="height: 400px; width: 400px" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="3" img-src="~assets/bg-3.jpg">
      <div class="absolute-center">
        <div class="text-white q-mt-xl text-center">
          <div class="text-h2">Our Signature</div>
          <div class="text-h1 text-weight-bold">Lx Movement</div>
          <div class="text-h6 text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem
            assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
            consequuntur quas nulla.
          </div>
          <br />
          <div class="text-h6 text-white">Learn More</div>
        </div>
      </div>
    </q-carousel-slide>
  </q-carousel>
  <q-carousel class="lt-sm" style="height: 100vh" animated v-model="slide" navigation>
    <q-carousel-slide :name="1" img-src="~assets/bg-1.jpg">
      <div class="row q-mt-sm">
        <div class="col-md-6 col-sm-12 col-xs-12 q-pt-sm" align="center">
          <q-img class="q-mt-md" src="~assets/item-1-1.png" style="height: 200px; width: 200px" />
        </div>
        <div class="col-md-6 col-sm-12 col-xs-12 text-white" align="left">
          <div class="text-h6">Sky-challanger</div>
          <div class="text-h4 text-weight-bold">Limited Edition</div>
          <div class="text-body2 text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem
            assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
            consequuntur quas nulla.
          </div>
          <br />
          <q-btn class="text-body1 q-pl-none" flat label="Learn More" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="2" img-src="~assets/bg-2.jpg">
      <div class="row q-mt-sm">
        <div class="col-md-6 col-sm-12 col-xs-12 q-my-sm text-white" align="center">
          <div class="text-h6 q-mb-md q-mt-sm text-weight-bold">Sport Series</div>
          <div class="text-body2 text-weight-light">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
            neque velit atque eius temporibus incidunt repudiandae quidem
            assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
            consequuntur quas nulla.
          </div>
          <br />
          <q-btn class="text-subtitle2 q-pl-none" flat label="Learn More" />
        </div>
        <div class="col-md-6 col-sm-12 col-xs-12 q-mt-xl" align="center">
          <q-img class="q-mt-xl" src="~assets/item-2-2.png" style="height: 200px; width: 200px" />
        </div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide :name="3" img-src="~assets/bg-3.jpg">
      <div class="text-white q-mt-sm text-center q-mt-lg">
        <div class="text-h5">Our Signature</div>
        <div class="text-h4 text-weight-bold">Lx Movement</div>
        <div class="text-body1 text-weight-light">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ut ipsa
          neque velit atque eius temporibus incidunt repudiandae quidem
          assumenda ratione ex reprehenderit iste non tempore, sequi voluptas
          consequuntur quas nulla.
        </div>
        <br />
        <div class="text-subtitle2 text-white">Learn More</div>
      </div>
    </q-carousel-slide>
  </q-carousel>
  <!-- ---------------------------- -->
  <div class="gt-xs row bg-brown-9 text-white q-px-xl q-col-gutter-md q-py-md">
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service1.jpg">
        <q-card-section>
          <div class="text-h5 text-warning text-weight-bold">
            PHARETRA NULLAM EUISMOD
          </div>
          <div class="text-h6 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service2.jpg">
        <q-card-section>
          <div class="text-h5 text-warning text-weight-bold">
            ORNARE RIDICULUS IPSUM
          </div>
          <div class="text-h6 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service3.jpg">
        <q-card-section>
          <div class="text-h5 text-warning text-weight-bold">
            PORTA AENEAN TRISTIQUE
          </div>
          <div class="text-h6 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
  <div class="lt-sm row bg-brown-9 text-white q-px-md q-col-gutter-md q-py-md">
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service1.jpg">
        <q-card-section>
          <div class="text-subtitle1 text-warning text-weight-bold">
            PHARETRA NULLAM EUISMOD
          </div>
          <div class="text-body2 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service2.jpg">
        <q-card-section>
          <div class="text-subtitle1 text-warning text-weight-bold">
            ORNARE RIDICULUS IPSUM
          </div>
          <div class="text-body2 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-md-4 col-sm-12 col-xs-12">
      <q-card flat class="my-card bg-transparent">
        <img src="~assets/column-service3.jpg">
        <q-card-section>
          <div class="text-subtitle1 text-warning text-weight-bold">
            PORTA AENEAN TRISTIQUE
          </div>
          <div class="text-body2 text-weight-light">
            Morbi leo risus, porta ac consectetur ac feanumi vestibulum at eros.
            Fusce dapibus, tellus ac cursus commodo, tortor mauris.
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
  <!-- ----------------------- -->
  <q-img class="gt-xs" src="~assets/SharedScreensh2ot.jpg" style="height: 600px" />
  <q-img class="lt-sm" src="~assets/SharedScreensh2ot.jpg" style="height: 300px" />
  <!-- ----------------------- -->
  <div class="row bg-positive gt-xs">
    <div class="col-1"></div>
    <div class="col-5 q-mt-lg" style="text-align: right">
      <div class="text-h5 text-warning">All Our Watches</div>
      <div class="text-h6 text-white">WE USE THE LATEST TECHNOLOGY</div>
      <div class="text-body1 text-grey-8">
        Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Fusce
        dapibus tellus ac cursus commodo, tortor mauris condimentum nibh, ut
        fermentum massa justo sit amet risus. Lorem ipsum dolor sit amet,
        consectetur. Praesent commodo cursus magna, vel scelerisque nisl
        consectetur.
      </div>
      <br />
      <div class="text-h6 text-warning">Learn More</div>
    </div>
    <div class="col-5">
      <q-img src="~assets/featured-image.jpg" />
    </div>
    <div class="col-1"></div>
  </div>
  <div class="row bg-positive lt-sm">
    <div class="col-md-6 col-sm-12 col-xs-12 q-mt-lg q-pr-md" style="text-align: right">
      <div class="text-h5 text-warning">All Our Watches</div>
      <div class="text-h6 text-white">WE USE THE LATEST TECHNOLOGY</div>
      <div class="text-body1 text-grey-8">
        Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Fusce
        dapibus tellus ac cursus commodo, tortor mauris condimentum nibh, ut
        fermentum massa justo sit amet risus. Lorem ipsum dolor sit amet,
        consectetur. Praesent commodo cursus magna, vel scelerisque nisl
        consectetur.
      </div>
      <br />
      <div class="text-h6 text-warning">Learn More</div>
    </div>
    <div class="col-md-6 col-sm-12 col-xs-12">
      <q-img src="~assets/featured-image.jpg" />
    </div>
    <div class="col-1"></div>
  </div>
  <!-- ----------------------- -->
  <div class="text-h4 text-grey-8 q-mt-md" style="text-align: center">
    Latest product
    <div class="text-body1 q-mt-md text-warning">
      View All Watches <q-icon name="fas fa-arrow-right"></q-icon>
    </div>
  </div>
  <!-- for slideshow smal -->
  <div class="q-pa-lg">
    <q-carousel v-model="slide" transition-prev="slide-right" transition-next="slide-left" swipeable animated
      control-color="primary" navigation padding arrows infinite height="300px" class="bg-secondary gt-xs">
      <q-carousel-slide :name="1" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-md q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height" src="~assets/photodune-1059393-mans-watch-m-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-4-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-2-400x250.jpg" />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="2" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-md q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-3-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-2-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-4-400x250.jpg" />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="3" class="column no-wrap">
        <div class="
            row
            fit
            justify-start
            items-center
            q-gutter-md q-col-gutter
            no-wrap
          ">
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-2-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height" src="~assets/photodune-1059393-mans-watch-m-400x250.jpg" />
          <q-img class="rounded-borders col-4 full-height"
            src="~assets/photodune-1659452-four-watches-m-2-400x250.jpg" />
        </div>
      </q-carousel-slide>

    </q-carousel>
    <q-carousel animated v-model="slides" arrows navigation infinite class="lt-sm">
      <q-carousel-slide :name="1" img-src="~assets/photodune-1659452-four-watches-m-2-400x250.jpg" style="width:100%" />
      <q-carousel-slide :name="2" img-src="~assets/photodune-1059393-mans-watch-m-400x250.jpg" style="width:100%" />
      <q-carousel-slide :name="3" img-src="~assets/photodune-1659452-four-watches-m-3-400x250.jpg" style="width:100%" />
      <q-carousel-slide :name="4" img-src="~assets/photodune-1659452-four-watches-m-4-400x250.jpg" style="width:100%" />
    </q-carousel>
  </div>
  <!-- ------------for about----------------- -->
  <q-img class="gt-xs" src="~assets/about-bg.jpg">
    <div class="row bg-transparent">
      <div class="col-md-6 col-sm-12 col-xs-12 flex flex-center">
        <div class="section text-center">
          <div class="text-h2 q-px-xl q-pt-xl text-weight-bold">
            A little about Us
          </div>
          <br />
          <div class="text-h6 q-mt-xl text-grey-8">
            Inspiration Can Be Found Everywhere
          </div>
        </div>
      </div>
      <div class="col-md-6 col-sm-12 col-xs-12 flex flex-center">
        <div class="section text-center">
          <div class="text-dark q-px-xl q-pt-xl text-grey-7">
            Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Fusce
            dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut
            fermentum massa justo sit amet risus. Lorem ipsum dolor sit amet,
            consectetur adipiscing elit. Donec id elit non mi porta gravida at eget
            metus. Praesent commodo cursus magna, vel scelerisque nisl consectetur
            et. Vestibulum id ligula porta felis euismod semper. Vivamus sagittis
            lacus vel augue laoreet rutrum faucibus dolor auctor. Vestibulum id
            ligula porta felis.
          </div>
        </div>
      </div>
    </div>
  </q-img>
  <!-- ----------------------------- -->
  <q-img class="gt-xs" src="~assets/award-bg.jpg">
    <div class="
        text-h2 text-accent text-weight-bold
        absolute-center
        bg-transparent
      ">
      AWARD WINNING
      <br />
      <div class="text-h6 q-mt-lg text-warning" style="text-align: center">
        Geneva, 2014
      </div>
    </div>
  </q-img>
  <q-img class="lt-sm" src="~assets/award-bg.jpg">
    <div class="
        text-subtitle1 text-accent text-weight-bold
        absolute-center
        bg-transparent
      ">
      AWARD WINNING
      <br />
      <div class="text-body2 text-warning" style="text-align: center">
        Geneva, 2014
      </div>
    </div>
  </q-img>
  <!-- ----------------------------- -->
  <div class="row bg-black">
    <div class="col-md-6 col-sm-12 col-xs-12">
      <div class="q-my-md">
        <div class="text-h4 text-white" style="text-align: center">
          Video Tour
        </div>
        <div class="text-h6 q-my-md text-warning" style="text-align: center">
          Small caption here
        </div>
      </div>
      <q-img src="~assets/ShdScreenshot.jpg">
        <div class="absolute-right q-gutter-md">
          <q-icon name="fas fa-heart" />
          <q-icon name="fas fa-share" />
        </div>
      </q-img>
    </div>
    <div class="col-md-6 col-sm-12 col-xs-12">
      <div class="q-my-md">
        <div class="text-h4 text-white" style="text-align: center">
          RECENT NEWS
        </div>
        <div class="text-body1 q-mt-md text-warning" style="text-align: center">
          Read All News <q-icon name="fas fa-arrow-right"></q-icon>
        </div>
      </div>
      <div class="gt-xs">
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="150px" src="~assets/photodune-2650397-sailing-m-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-h6 text-white q-ml-md">
                SEM PORTA MOLLIS PARTURIENT
              </div>
              <div class="text-h6 text-white q-mx-md">
                <q-icon name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="150px" src="~assets/photodune-1892957-gear-m-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-h6 text-white q-ml-md">
                NULLAM LOREM MATTIS PURUS
              </div>
              <div class="text-h6 text-white q-mx-md">
                <q-icon name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="150px" src="~assets/Fotolia_42598149_Subscription_Monthly_XXL-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-h6 text-white q-ml-md">
                NIBH SEM SIT ULLAMCORPER
              </div>
              <div class="text-h6 text-white q-mx-md">
                <q-icon name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
      </div>
      <div class="lt-sm">
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="100px" src="~assets/photodune-2650397-sailing-m-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-subtitle2 text-white q-ml-md">
                SEM PORTA MOLLIS PARTURIENT
              </div>
              <div class="text-subtitle2 text-white q-mx-md text-weight-light">
                <q-icon class="q-mr-sm" name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="100px" src="~assets/photodune-1892957-gear-m-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-subtitle2 text-white q-ml-md">
                NULLAM LOREM MATTIS PURUS
              </div>
              <div class="text-subtitle2 text-white q-mx-md text-weight-light">
                <q-icon class="q-mr-sm" name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
        <q-list>
          <q-item>
            <q-item-section avatar>
              <q-img width="100px" src="~assets/Fotolia_42598149_Subscription_Monthly_XXL-150x150.jpg"> </q-img>
            </q-item-section>
            <q-item-section>
              <div class="text-subtitle2 text-white q-ml-md">
                NIBH SEM SIT ULLAMCORPER
              </div>
              <div class="text-subtitle2 text-white q-mx-md text-weight-light">
                <q-icon class="q-mr-sm" name="fas fa-clock"></q-icon>21 Mar 2014
              </div>
            </q-item-section>
          </q-item>
        </q-list>
      </div>
    </div>
  </div>
  <!-- ------------for footer----------------- -->
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
  <!-- ----------------------------- -->
</template>

<script>
import { ref } from "vue";
export default {
  data() {
    return {
      slide: ref(1),
      slides: ref(1)
    };
  },
};
</script>


<style lang="scss">
.section {
  display: grid;
  justify-content: center;
  align-content: center;
}
</style>
