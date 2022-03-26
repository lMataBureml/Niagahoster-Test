<template>
  <div>
    <q-header>
      <q-toolbar
        class="row full-width items-center justify-between"
        style="
          height: 80px;
          background-color: #0094ff;
          background: linear-gradient(to right, #0094ff, #007aff, #026ce8);
          padding: 0px 40px 0px 40px;
        "
      >
        <div class="col-3">
          <q-img
            style="cursor: pointer"
            @click="$router.push('/')"
            no-spinner
            width="80%"
            src="~assets/Niagahoster-Logo.png"
          ></q-img>
        </div>
        <div class="col-6">
          <div
            class="row justify-center"
            style="font-family: Nunito SansSemi; font-size: 16px"
          >
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white">Hosting</a>
            </div>
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white">VPS</a>
            </div>
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white">Domain</a>
            </div>
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white"
                >Kemitraan</a
              >
            </div>
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white">Wawasan</a>
            </div>
            <div class="col" style="text-align: center">
              <a href="" style="text-decoration: none; color: white">Acara</a>
            </div>
          </div>
        </div>
        <div class="col-3" style="text-align: right">
          <q-toolbar class="justify-end">
            <div class="q-ma-lg">
              <q-icon name="fas fa-light fa-cart-shopping" size="16px"></q-icon>
            </div>
            <div>
              <q-btn-dropdown
                unelevated
                dense
                style="
                  color: white;
                  font-family: Nunito SansSemi;
                  font-size: 16px;
                "
                label="ID"
                dropdown-icon="expand_more"
              >
                <q-list>
                  <q-item clickable v-close-popup>
                    <q-item-section>
                      <q-item-label>Indonesia</q-item-label>
                    </q-item-section>
                  </q-item>
                  <q-item clickable v-close-popup>
                    <q-item-section>
                      <q-item-label>English</q-item-label>
                    </q-item-section>
                  </q-item>
                </q-list>
              </q-btn-dropdown>
            </div>
            <div class="q-ml-md">
              <q-btn
                class="q-px-lg"
                unelevated
                rounded
                outline
                color="white"
                no-caps
                style="font-family: Nunito SansBold; font-size: 14px"
                >Login</q-btn
              >
            </div>
          </q-toolbar>
        </div>
      </q-toolbar>
    </q-header>
    <div class="container">
      <div
        class="SmallMenu row full-width justify-center items-center"
        style="height: 48px; background-color: #0057b2"
      >
        <div class="q-mx-md">
          <q-btn-dropdown
            unelevated
            dense
            no-caps
            style="color: white; font-family: Nunito SansSemi; font-size: 16px"
            label="Tutorial"
            dropdown-icon="expand_more"
          >
            <q-list style="background-color: #0057b2; color: white">
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Tutorial 1</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Tutorial 2</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </div>
        <div class="q-mx-md">
          <q-btn-dropdown
            unelevated
            dense
            no-caps
            style="color: white; font-family: Nunito SansSemi; font-size: 16px"
            label="Digital Marketing"
            dropdown-icon="expand_more"
          >
            <q-list style="background-color: #0057b2; color: white">
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Manfaat</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Produk</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </div>
        <div class="q-mx-md">
          <q-btn-dropdown
            unelevated
            dense
            no-caps
            style="color: white; font-family: Nunito SansSemi; font-size: 16px"
            label="Web Development & Design"
            dropdown-icon="expand_more"
          >
            <q-list style="background-color: #0057b2; color: white">
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Design</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Produk</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </div>
        <div class="q-mx-md">
          <q-btn-dropdown
            unelevated
            dense
            no-caps
            style="color: white; font-family: Nunito SansSemi; font-size: 16px"
            label="Insight Bisnis"
            dropdown-icon="expand_more"
          >
            <q-list style="background-color: #0057b2; color: white">
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Pemahaman</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Buku</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </div>
        <div class="q-mx-md">
          <q-btn-dropdown
            unelevated
            dense
            no-caps
            style="color: white; font-family: Nunito SansSemi; font-size: 16px"
            label="News & Updates"
            dropdown-icon="expand_more"
          >
            <q-list style="background-color: #0057b2; color: white">
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Berita</q-item-label>
                </q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Artikel</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </div>
      </div>
      <div
        class="BigHighlight row justify-center q-pt-xl"
        style="
          height: 506px;
          background-color: #0094ff;
          background: linear-gradient(to right, #0094ff, #007aff, #026ce8);
        "
      >
        <div class="WrapBox" style="text-align: center">
          <div
            class="BigText"
            style="font-family: Nunito SansBold; font-size: 56px; color: white"
          >
            <div style="margin-bottom: -5px">Dapatkan Artikel</div>
            <div
              id="flip"
              style="height: 60px; overflow: hidden; margin-bottom: -5px"
            >
              <div><div>Tutorial Hosting</div></div>
              <div><div>Tutorial Website</div></div>
              <div><div>Digital Marketing</div></div>
              <div><div>Tutorial Design Website</div></div>
            </div>
            <div>Terbaik Disini</div>
          </div>
          <div
            class="LittleText q-mt-lg"
            style="
              font-family: Nunito SansNormal;
              color: white;
              font-size: 16px;
            "
          >
            Temukan artikel berisi solusi terbaik untuk segala permasalahan Anda
          </div>
          <q-input
            rounded
            outlined
            borderless
            v-model="text"
            class="q-mt-xl"
            bg-color="white"
            label="Cari topic artikel yang ingin Anda cari . . ."
            style="font-family: Nunito SansNormal; font-size: 16px"
          >
            <template v-slot:append>
              <q-icon name="search" v-if="text === ''" />
              <q-icon
                v-else
                name="clear"
                class="cursor-pointer"
                @click="text = ''"
              />
            </template>
          </q-input>
        </div>
      </div>
      <div class="BodyPage q-mx-xl" style="margin-top: 60px">
        <div class="row justify-center">
          <div class="col-7 q-pr-lg">
            <div
              class="JudulTerbaru items-center q-mb-lg"
              style="display: flex"
            >
              <q-img no-spinner width="50px" src="~assets/Terbaru.png"></q-img>
              <div
                class="q-ml-lg"
                style="
                  font-family: Nunito SansBold;
                  font-size: 32px;
                  color: #29384e;
                "
              >
                Artikel Terbaru
              </div>
            </div>
            <div class="ListArtikelBaru">
              <div v-for="n in 3" :key="n">
                <artikel-terbaru></artikel-terbaru>
              </div>
            </div>
            <div
              class="q-my-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                text-align: center;
              "
            >
              <a href="" style="text-decoration: none; color: #007aff"
                >Lihat Semua Artikel</a
              >
            </div>
            <div class="Jeda q-my-md" style="height: 40px"></div>
            <div
              class="JudulTerpopuler items-center q-mb-lg"
              style="display: flex"
            >
              <q-img
                no-spinner
                width="50px"
                src="~assets/Terpopuler.png"
              ></q-img>
              <div
                class="q-ml-lg"
                style="
                  font-family: Nunito SansBold;
                  font-size: 32px;
                  color: #29384e;
                "
              >
                Artikel Populer
              </div>
            </div>
            <div class="ListArtikelPopuler">
              <div v-for="n in 3" :key="n">
                <artikel-terbaru></artikel-terbaru>
              </div>
            </div>
            <div
              class="q-my-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                text-align: center;
              "
            >
              <a href="" style="text-decoration: none; color: #007aff"
                >Lihat Semua Artikel</a
              >
            </div>
            <div class="Jeda q-my-md" style="height: 40px"></div>
            <div
              class="MiddleBox row full-width q-pa-lg items-center"
              style="
                background-color: #0094ff;
                background: linear-gradient(
                  to right,
                  #0094ff,
                  #007aff,
                  #026ce8
                );
                border-radius: 15px;
              "
            >
              <div class="col-6 q-px-md">
                <div
                  style="
                    font-family: Nunito SansBold;
                    color: white;
                    font-size: 24px;
                  "
                >
                  Ingin jadi yang pertama tau artikel terbaru kami?
                </div>
                <div
                  class="q-mt-lg"
                  style="
                    font-family: Nunito SansNormal;
                    color: white;
                    font-size: 16px;
                  "
                >
                  Kami akan mengirimkan pemberitahuan artikel terbaru kami
                  melalui email Anda. Ingin mendapatkan pemberitahuan?
                </div>
              </div>
              <div class="col-6 q-px-md" style="text-align: center">
                <q-btn
                  no-caps
                  rounded
                  dense
                  color="orange"
                  text-color="white"
                  style="
                    font-family: Nunito SansBold;
                    font-size: 20px;
                    width: 100%;
                  "
                >
                  Langganan Sekarang
                </q-btn>
              </div>
            </div>
            <div
              class="Semua Artikel q-mb-md q-mt-xl"
              style="
                font-family: Nunito SansBold;
                font-size: 32px;
                color: #29384e;
              "
            >
              Semua Artikel
            </div>
            <div class="ListSemuaArtikel row justify-center">
              <div class="col-4 q-mb-lg" v-for="n in 3" :key="n">
                <semua-artikel></semua-artikel>
              </div>
              <div class="col-4 q-mb-lg" v-for="n in 3" :key="n">
                <semua-artikel></semua-artikel>
              </div>
              <div class="col-4 q-mb-lg" v-for="n in 3" :key="n">
                <semua-artikel></semua-artikel>
              </div>
            </div>
            <div
              class="row justify-center q-mb-xl"
              style="
                font-family: Nunito SansSemi;
                font-size: 16px;
                color: #29384e;
              "
            >
              <div
                class="PageBack col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                <q-icon name="fa-solid fa-chevron-left" />
              </div>
              <div
                class="PageOne col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                1
              </div>
              <div
                class="PageTwo col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                2
              </div>
              <div
                class="PageThree col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                3
              </div>
              <div
                class="PageBack col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                <q-icon name="fa-solid fa-ellipsis" />
              </div>
              <div
                class="PageThreen col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                13
              </div>
              <div
                class="PageBack col-2 q-pa-sm q-mx-sm"
                style="
                  cursor: pointer;
                  height: 40px;
                  width: 40px;
                  border-radius: 10px;
                  outline: #d9dde3 solid 2px;
                  text-align: center;
                "
              >
                <q-icon name="fa-solid fa-chevron-right" />
              </div>
            </div>
          </div>
          <div class="col-3 q-pb-xl">
            <div class="SideMenu" style="position: sticky; top: 140px">
              <q-input
                class="q-pl-lg"
                outlined
                rounded
                label="Cari artikel blog..."
              >
                <template v-slot:append>
                  <q-icon name="search" v-if="text === ''" />
                  <q-icon
                    v-else
                    name="clear"
                    class="cursor-pointer"
                    @click="text = ''"
                  />
                </template>
              </q-input>
              <div class="SideMenuList q-pa-lg">
                <div
                  class="q-mt-lg q-mb-lg q-ml-md"
                  style="
                    font-family: Nunito SansBold;
                    font-size: 20px;
                    color: #29384e;
                  "
                >
                  Kategori Blog
                </div>
                <!-- <q-btn-dropdown
                  flat
                  no-caps
                  style="
                    font-family: Nunito SansSemi;
                    font-size: 14px;
                    color: #29384e;
                  "
                  label="Tutorial"
                  dropdown-icon="expand_more"
                >
                  <q-list>
                    <q-item> </q-item>
                  </q-list>
                </q-btn-dropdown> -->
                <q-list
                  style="
                    font-family: Nunito SansSemi;
                    font-size: 14px;
                    color: #29384e;
                  "
                >
                  <q-expansion-item
                    group="Sidemenu"
                    label="Tutorial"
                    style="padding-left: 0px"
                  >
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Tutorial 1
                    </div>
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Tutorial 2
                    </div>
                  </q-expansion-item>
                  <q-expansion-item group="Sidemenu" label="Digital Marketing">
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Digital Marketing 1
                    </div>
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Digital Marketing 1
                    </div>
                  </q-expansion-item>
                  <q-expansion-item
                    group="Sidemenu"
                    label="Web Development & Design"
                  >
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Website 1
                    </div>
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Website 2
                    </div>
                  </q-expansion-item>
                  <q-expansion-item group="Sidemenu" label="Insight Bisnis">
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Insight 1
                    </div>
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Insight 2
                    </div>
                  </q-expansion-item>
                  <q-expansion-item group="Sidemenu" label="News & Update">
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      News
                    </div>
                    <div
                      class="q-pl-md q-py-sm"
                      style="background-color: #f5f5f5"
                    >
                      Update
                    </div>
                  </q-expansion-item>
                </q-list>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="BottomBox full-width q-pa-xl"
        style="
          background-color: #0094ff;
          background: linear-gradient(to right, #0094ff, #007aff, #026ce8);
          text-align: center;
        "
      >
        <div
          class="q-py-lg"
          style="font-family: Nunito SansBold; color: white; font-size: 40px"
        >
          Awali Kesuksesan Anda Bersama Niagahoster
        </div>
        <div class="row justify-center">
          <div
            class="col-6 q-my-sm"
            style="
              font-family: Nunito SansNormal;
              color: white;
              font-size: 16px;
            "
          >
            Kini tidak lagi sulit mewujudkan website impian. Performa hebat,
            keamanan ekstra, dan layanan dukungan teknis yang bisa diandalkan -
            semua dengan harga terjangkau!
          </div>
        </div>
        <div class="row justify-center">
          <div class="col-3 q-py-xl" style="text-align: center">
            <q-btn
              no-caps
              type="a"
              href="https://www.niagahoster.co.id/"
              rounded
              dense
              color="orange"
              text-color="white"
              style="font-family: Nunito SansBold; font-size: 20px; width: 100%"
            >
              Mulai Sekarang
            </q-btn>
          </div>
        </div>
      </div>
    </div>
    <div
      class="Footer q-pa-xl"
      style="background-color: #22273c; height: 982px"
    >
      <div class="row q-py-md justify-evenly">
        <div class="col-2 q-mt-lg">
          <div class="Box1">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Web Hosting
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Hosting Indonesia
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Cloud Indonesia
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Email Indonesia
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Web Hosting Unlimited
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Hosting Terbaik
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Hosting Murah
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Hosting Singapore SG
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Keamanan SSL/HTTPS
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Data Center Hosting Terbaik
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Hosting Gratis
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Transfer Hosting
            </div>
          </div>
          <div class="Box2 q-pt-lg">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Domain
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Domain
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Domain .ID
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Domain Gratis
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Promosi Domain .COM
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              WHOIS
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Transfer Domain
            </div>
          </div>
        </div>
        <div class="col-2 q-mt-lg">
          <div class="Box3">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Virtual Private Server
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              VPS KVM Indonesia
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Cloud VPS Hosting
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              CyberPanel VPS Hosting
            </div>
          </div>
          <div class="Box4 q-pt-lg">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              WordPress Hosting
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              WordPress Hosting
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Managed WordPress
            </div>
          </div>
          <div class="Box5 q-pt-lg">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Website
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Website Instan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Jasa Pembuatan Website
            </div>
          </div>
          <div class="Box6 q-pt-lg">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Bantuan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Cara Pembayaran
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Ebook Gratis
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Knowledge Base
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Blog
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Course
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Forum
            </div>
          </div>
        </div>
        <div class="col-2 q-mt-lg">
          <div class="Box7">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Kemitraan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Poin
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Partner
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Program Afiliasi Niagahoster
            </div>
          </div>
          <div class="Box8 q-pt-lg">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Perusahaan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Tentang Niagahoster
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Kontak
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Karir
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Event
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Status Layanan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Review Pelanggan
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Penawaran & Promo Spesial
            </div>
            <div
              class="q-mb-md"
              style="
                font-family: Nunito SansNormal;
                font-size: 14px;
                color: #a9afb8;
              "
            >
              Niagahoster Virtual Summit
            </div>
          </div>
          <div class="Box9" style="padding-top: 55%; width: 220%">
            <div
              class="q-mb-lg"
              style="
                font-family: Nunito SansBold;
                font-size: 16px;
                color: white;
              "
            >
              Newsletter
            </div>
            <div class="row">
              <div class="col-7">
                <q-input
                  rounded
                  dense
                  outlined
                  borderless
                  v-model="text"
                  flat
                  bg-color="white"
                  label="Write your input here"
                  label-color="#A9AFB8"
                  style="font-family: Nunito SansNormal; font-size: 16px"
                >
                </q-input>
              </div>
              <div class="col-3 q-ml-md">
                <q-btn
                  class="q-px-lg"
                  rounded
                  no-caps
                  color="orange"
                  style="Nunito SansBold;font-size:16px;color:white"
                  >Berlangganan</q-btn
                >
              </div>
            </div>
          </div>
        </div>
        <div class="col-3 q-mt-lg q-mb-xl">
          <div class="Box10">
            <div>
              <q-img
                no-spinner
                src="~assets/Niagahoster-Logo2.png"
                style="
                  object-fit: cover;
                  width: 80%;
                  height: 90%;
                  border-radius: 5px;
                "
              ></q-img>
              <div
                class="q-pr-xl q-pt-xl"
                style="
                  font-family: Nunito SansNormal;
                  font-size: 14px;
                  color: white;
                "
              >
                Misi kami adalah membantu jutaan orang memanfaatkan potensi yang
                ada di internet untuk membangun kesuksesan online.
              </div>
              <div
                class="q-pr-xl q-pt-xl"
                style="
                  font-family: Nunito SansNormal;
                  font-size: 14px;
                  color: white;
                "
              >
                Jl. Palagan Tentara Pelajar No 81 Jongkang, Sariharjo, Ngaglik,
                Sleman Daerah Istimewa Yogyakarta 55581
              </div>
              <div
                class="q-pr-xl q-pt-xl"
                style="
                  font-family: Nunito SansNormal;
                  font-size: 14px;
                  color: white;
                "
              >
                <div>Telepon: 0274-2885822</div>
                <div>WhatsApp: 085943258274</div>
                <div>Telegram: @niagahost_bot</div>
              </div>
              <div class="BoxMedsos row q-mt-xl">
                <div class="col-2">
                  <div
                    class=""
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-facebook-f"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                  <div
                    class="q-mt-lg"
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-twitter"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                </div>
                <div class="col-2 q-pl-sm">
                  <div
                    class=""
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-instagram"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                  <div
                    class="q-mt-lg"
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-tiktok"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                </div>
                <div class="col-2 q-pl-md">
                  <div
                    class=""
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-linkedin"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                  <div
                    class="q-mt-lg"
                    style="
                      display: flex;
                      align-items: center;
                      justify-content: center;
                      height: 48px;
                      width: 48px;
                      background-color: #546071;
                      border-radius: 100%;
                    "
                  >
                    <q-icon
                      name="fa-brands fa-youtube"
                      size="1.5em"
                      color="white"
                    />
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div
          class="row q-mt-xl q-pt-lg justify-between"
          style="border-top: 2px solid #546071"
        >
          <div
            class="col-7"
            style="
              font-family: Nunito SansNormal;
              font-size: 12px;
              color: white;
            "
          >
            Copyright ©2021 Niagahoster | Hosting powered by PHP8, CloudLinux,
            CloudFlare, BitNinja and DC DCI-Indonesia | Cloud VPS Murah powered
            by Webuzo Softaculous, Intel SSD and cloud computing technologys
          </div>
          <div
            class="col-3"
            style="
              font-family: Nunito SansNormal;
              font-size: 12px;
              color: white;
              display: flex;
              justify-content: flex-end;
            "
          >
            <div class="q-pr-sm">Syarat dan Ketentuan</div>
            <div
              style="
                margin-top: 2px;
                width: 1px;
                height: 14px;
                background-color: white;
              "
            ></div>
            <div class="q-pl-sm">Kebijakan Privasi</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArtikelTerbaru from "components/ArtikelTerbaru.vue";
import SemuaArtikel from "components/SemuaArtikel.vue";
export default {
  components: {
    // ArtikelTerbaru: () => import("components/ArtikelTerbaru.vue"),
    ArtikelTerbaru,
    SemuaArtikel,
  },
};
</script>

<style></style>
