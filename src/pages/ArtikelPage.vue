<template>
  <div>
    <div>
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
              <q-icon
                color="white"
                name="fas fa-light fa-cart-shopping"
                size="16px"
              ></q-icon>
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
    </div>
    <q-drawer
      v-model="comment"
      :width="350"
      :breakpoint="500"
      side="right"
      overlay
      content-class="bg-white"
    >
      <q-scroll-area class="fit">
        <div class="q-px-xl q-pt-xl q-pb-md">
          <div class="row justify-between">
            <div class="col-6 items-center" style="display: flex">
              <q-icon name="chat" color="blue-grey-9" size="2.2em"></q-icon>
              <div
                class="q-mx-md"
                style="
                  font-family: Nunito SansBold;
                  font-size: 20px;
                  color: #29384e;
                "
              >
                Balasan
              </div>
              <div
                class=""
                style="
                  font-family: Nunito SansBold;
                  font-size: 20px;
                  color: #007aff;
                "
              >
                15
              </div>
            </div>
            <div
              class="col-2 items-center"
              style="display: flex; justify-content: flex-end"
            >
              <q-icon
                name="close"
                size="2.2em"
                clickable
                @click="comment = !comment"
                style="cursor: pointer"
              ></q-icon>
            </div>
          </div>
          <div
            class="q-my-lg q-pa-md"
            style="outline: 1px solid #a9afb8; border-radius: 10px"
          >
            <q-input v-model="text" type="textarea"></q-input>
          </div>
        </div>
        <q-separator />
        <div class="q-my-xl q-px-xl">
          <div class="row">
            <div class="col-2 items-center">
              <q-img
                no-spinner
                src="~assets/Adam.png"
                style="object-fit: cover; width: 100%; height: 100%"
              ></q-img>
            </div>
            <div class="col q-ml-md">
              <div
                style="
                  font-family: Nunito SansSemi;
                  font-size: 16px;
                  color: #29384e;
                "
              >
                Adam Muiz
              </div>
              <div
                class="q-mt-xs"
                style="
                  font-family: Nunito SansNormal;
                  font-size: 12px;
                  color: #7f8895;
                "
              >
                29 Hari yang lalu
              </div>
            </div>
          </div>
          <div
            class="q-my-sm"
            style="
              font-family: Nunito SansNormal;
              font-size: 14px;
              color: #29384e;
            "
          >
            makasih kak udah berbagi informasi hehe
          </div>
          <div class="q-pt-sm" style="display: flex">
            <q-icon
              name="fa-regular fa-thumbs-up"
              color="blue-grey-7"
              size="1.8em"
            ></q-icon>
            <q-icon
              size="1.8em"
              class="q-ml-md"
              name="fa-solid fa-reply"
              color="blue-grey-7"
            ></q-icon>
          </div>
        </div>
        <q-separator />
      </q-scroll-area>
    </q-drawer>
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
      <div class="BodyPageArtikel q-mt-sm">
        <div class="row justify-center q-mb-xl q-px-xl">
          <div class="col-10">
            <div class="row justify-center q-py-xl">
              <div class="col-3">
                <div
                  class="Sidemenu q-pr-xl"
                  style="position: sticky; top: 20px; margin-top: 610px"
                >
                  <div
                    class="HistoryPage items-center q-mb-lg"
                    style="
                      display: flex;
                      font-family: Nunito SansNormal;
                      font-size: 12px;
                    "
                  >
                    <div class="" style="color: #007aff">Home</div>
                    <q-icon
                      class="q-px-md"
                      name="fa-solid fa-chevron-right"
                      color="black"
                      size="0.8em"
                    ></q-icon>
                    <div class="" style="color: #007aff">Tutorial</div>
                    <q-icon
                      class="q-px-md"
                      name="fa-solid fa-chevron-right"
                      color="black"
                      size="0.8em"
                    ></q-icon>
                    <div class="" style="color: #007aff">Hosting</div>
                  </div>
                  <div
                    class="JudulArtikel q-mb-md"
                    style="
                      font-family: Nunito SansBold;
                      font-size: 20px;
                      color: #29384e;
                    "
                  >
                    4+ Cara Mudah Cek IP Hosting Website
                  </div>
                  <div class="items-center q-mb-md" style="display: flex">
                    <q-img
                      no-spinner
                      style="object-fit: cover; width: 20px; height: 20px"
                      src="~assets/Foto.png"
                    ></q-img>
                    <div
                      class="q-ml-md"
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: #29384e;
                      "
                    >
                      Nida Regita F
                    </div>
                  </div>
                  <div class="items-center" style="display: flex">
                    <div
                      class=""
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: ##546071;
                      "
                    >
                      28 Dec 2021
                    </div>
                    <div
                      class="q-mx-md"
                      style="
                        width: 5px;
                        height: 5px;
                        border-radius: 100%;
                        background-color: #29384e;
                      "
                    ></div>
                    <div
                      class=""
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: ##546071;
                      "
                    >
                      5 min read
                    </div>
                  </div>
                  <div
                    class="q-my-lg"
                    style="height: 1px; background-color: #d9dde3"
                  ></div>
                  <div class="" style="display: flex">
                    <q-icon
                      name="fa-regular fa-thumbs-up"
                      color="blue-grey-7"
                      size="1.4em"
                    ></q-icon>
                    <div class="q-pr-lg q-pl-sm">111</div>
                    <q-icon
                      clickable
                      @click="comment = !comment"
                      name="fa-solid fa-comment"
                      color="blue-grey-7"
                      size="1.4em"
                      style="cursor: pointer"
                    ></q-icon>
                    <div class="q-pl-sm q-pr-lg">4</div>
                    <q-icon
                      name="fa-solid fa-share-nodes"
                      color="blue-grey-7"
                      size="1.4em"
                    ></q-icon>
                    <div class="q-pl-sm">Share</div>
                  </div>
                </div>
              </div>
              <div class="col-7">
                <div
                  class="HistoryPage items-center q-mb-lg"
                  style="
                    display: flex;
                    font-family: Nunito SansNormal;
                    font-size: 12px;
                  "
                >
                  <div class="" style="color: #007aff">Home</div>
                  <q-icon
                    class="q-px-md"
                    name="fa-solid fa-chevron-right"
                    color="black"
                    size="0.8em"
                  ></q-icon>
                  <div class="" style="color: #007aff">Tutorial</div>
                  <q-icon
                    class="q-px-md"
                    name="fa-solid fa-chevron-right"
                    color="black"
                    size="0.8em"
                  ></q-icon>
                  <div class="" style="color: #007aff">Hosting</div>
                  <q-icon
                    class="q-px-md"
                    name="fa-solid fa-chevron-right"
                    color="black"
                    size="0.8em"
                  ></q-icon>
                  <div class="" style="color: ##546071">
                    4+ Cara Mudah Cek IP Hosting Website
                  </div>
                </div>
                <div
                  class="JudulArtikel q-mb-md"
                  style="
                    font-family: Nunito SansBold;
                    font-size: 40px;
                    color: #29384e;
                  "
                >
                  4+ Cara Mudah Cek IP Hosting Website
                </div>
                <div class="UserArtikel row q-mb-lg justify-between">
                  <div class="col-6 items-center" style="display: flex">
                    <q-img
                      no-spinner
                      style="object-fit: cover; width: 20px; height: 20px"
                      src="~assets/Foto.png"
                    ></q-img>
                    <div
                      class="q-ml-md"
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: #29384e;
                      "
                    >
                      Nida Regita F
                    </div>
                    <div
                      class="q-mx-md"
                      style="
                        width: 5px;
                        height: 5px;
                        border-radius: 100%;
                        background-color: #29384e;
                      "
                    ></div>
                    <div
                      class=""
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: ##546071;
                      "
                    >
                      28 Dec 2021
                    </div>
                    <div
                      class="q-mx-md"
                      style="
                        width: 5px;
                        height: 5px;
                        border-radius: 100%;
                        background-color: #29384e;
                      "
                    ></div>
                    <div
                      class=""
                      style="
                        font-family: Nunito SansNormal;
                        font-size: 12px;
                        color: ##546071;
                      "
                    >
                      5 min read
                    </div>
                  </div>
                  <div
                    class="col-5 items-center justify-end"
                    style="
                      display: flex;
                      font-family: Nunito SansSemi;
                      font-size: 12px;
                      color: #546071;
                    "
                  >
                    <q-icon
                      name="fa-regular fa-thumbs-up"
                      color="blue-grey-7"
                      size="1.6em"
                    ></q-icon>
                    <div class="q-pl-sm q-pr-lg">111</div>
                    <q-icon
                      clickable
                      @click="comment = !comment"
                      name="fa-solid fa-comment"
                      color="blue-grey-7"
                      size="1.6em"
                      style="cursor: pointer"
                    ></q-icon>
                    <div class="q-pl-sm q-pr-lg">4</div>
                    <q-icon
                      name="fa-solid fa-share-nodes"
                      color="blue-grey-7"
                      size="1.6em"
                    ></q-icon>
                    <div class="q-pl-sm">Share</div>
                  </div>
                </div>
                <q-img
                  class="q-mt-sm q-mb-xl"
                  no-spinner
                  src="~assets/Image-Full.png"
                  style="object-fit: cover; width: 100%; border-radius: 10px"
                />
                <div
                  class="q-mb-md"
                  style="
                    font-family: Nunito SansNormal;
                    font-size: 18px;
                    color: #29384e;
                  "
                >
                  Anda ingin tahu cara cek IP hosting? Selamat, Anda berada di
                  halaman yang tepat! IP hosting adalah barisan angka sebagai
                  identitas unik dari suatu hosting website. Dengan IP tersebut,
                  website Anda dapat dikenali dan diakses melalui jaringan
                  internet. Saat Anda mengakses website, Anda memang tidak bisa
                  melihat IP secara langsung. Alasannya, IP tersebut sudah
                  diwakili oleh sebuah domain agar lebih mudah diingat. Kalau
                  begitu, bagaimana cara mengetahui hosting IP suatu website?
                  Yuk, simak panduan lengkap cara cek IP web hosting di bawah
                  ini!
                </div>
                <q-list
                  bordered
                  class="q-py-lg q-px-md q-mb-lg"
                  style="border-radius: 10px"
                >
                  <q-expansion-item
                    default-opened
                    group="DaftarIsi"
                    label="Daftar Isi"
                    style="
                      font-family: Nunito SansBold;
                      font-size: 20px;
                      color: #29384e;
                    "
                  >
                    <div
                      class="q-mt-lg q-mb-md q-pl-md"
                      style="font-size: 12px; color: #007aff; cursor: pointer"
                    >
                      Cara Cek IP Hosting
                    </div>
                    <div
                      class="q-mb-md q-pl-xl"
                      style="font-size: 12px; color: #007aff; cursor: pointer"
                    >
                      Melihat IP Hosting pada email informasi akun hosting
                    </div>
                    <div
                      class="q-mb-md q-pl-xl"
                      style="font-size: 12px; color: #29384e; cursor: pointer"
                    >
                      Melihat IP Hosting melalui Member Area Niagahoster
                    </div>
                    <div
                      class="q-mb-md q-pl-xl"
                      style="font-size: 12px; color: #29384e; cursor: pointer"
                    >
                      Melihat IP Hosting melalui cPanel
                    </div>
                    <div
                      class="q-mb-md q-pl-xl"
                      style="font-size: 12px; color: #29384e; cursor: pointer"
                    >
                      Melihat IP menggunakan CMD
                    </div>
                    <div
                      class="q-mb-lg q-pl-xl"
                      style="font-size: 12px; color: #29384e; cursor: pointer"
                    >
                      Melihat IP dengan web-based tools
                    </div>
                    <div
                      class="q-mb-md q-pl-md"
                      style="font-size: 12px; color: #29384e; cursor: pointer"
                    >
                      Kesimpulan
                    </div>
                  </q-expansion-item>
                </q-list>
                <div
                  class="q-mb-lg"
                  style="
                    font-family: Nunito SansBold;
                    font-size: 28px;
                    color: #29384e;
                  "
                >
                  Cara Cek IP Hosting
                </div>
                <div
                  class="q-mb-md"
                  style="
                    font-family: Nunito SansNormal;
                    font-size: 18px;
                    color: #29384e;
                  "
                >
                  Anda dapat melakukan cek IP hosting dengan berbagai cara,
                  diantaranya adalah: Melihat IP Hosting pada Email Informasi
                  Akun Hosting Melihat IP Hosting Melalui Member Area
                  Niagahoster Melihat IP Hosting Melalui cPanel Mengecek IP
                  Menggunakan CMD Mengecek IP dengan Web-based Tools Nah,
                  berikut ini penjelasan lengkapnya:
                </div>
                <div
                  class="q-mb-lg"
                  style="
                    font-family: Nunito SansBold;
                    font-size: 28px;
                    color: #29384e;
                  "
                >
                  1. Melihat IP Hosting pada Email Informasi Akun Hosting
                </div>
                <div
                  class="q-mb-xl"
                  style="
                    font-family: Nunito SansNormal;
                    font-size: 18px;
                    color: #29384e;
                  "
                >
                  Ketika Anda membeli layanan hosting, pihak penyedia hosting
                  akan mengirimkan email berupa informasi detail akun hosting
                  Anda. Pada email ini, Anda bisa cek IP di bagian Informasi
                  Akun seperti ini:
                </div>
                <div
                  class="q-mb-xl TombolBerlangganan"
                  style="text-align: center"
                >
                  <q-btn
                    class="full-width"
                    unelevated
                    outline
                    rounded
                    color="orange"
                    no-caps
                    label="Berlangganan Hosting Niagahoster Sekarang Juga!"
                    style="font-family: Nunito SansBold; font-size: 20px"
                  >
                  </q-btn>
                </div>
                <div
                  class="row justify-between"
                  style="
                    font-family: Nunito SansSemi;
                    font-size: 20px;
                    color: #546071;
                  "
                >
                  <div class="col-4" style="display: flex">
                    <q-icon
                      name="fa-regular fa-thumbs-up"
                      color="blue-grey-7"
                      size="1.6em"
                    ></q-icon>
                    <div class="q-pr-lg q-pl-md">111</div>
                    <q-icon
                      clickable
                      @click="comment = !comment"
                      name="fa-solid fa-comment"
                      color="blue-grey-7"
                      size="1.6em"
                      style="cursor: pointer"
                    ></q-icon>
                    <div class="q-pr-lg q-pl-md">4</div>
                  </div>
                  <div
                    class="col-3"
                    style="display: flex; justify-content: flex-end"
                  >
                    <q-icon
                      name="fa-solid fa-share-nodes"
                      color="blue-grey-7"
                      size="1.6em"
                    ></q-icon>
                    <div class="q-px-md">Share</div>
                  </div>
                </div>
              </div>
              <div class="col-2"></div>
              <div class="q-py-xl"></div>
            </div>
            <div
              class="MiddleBox row full-width q-pa-lg items-center q-mb-xl"
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
          </div>
        </div>
        <div
          class="ArtikelTerkait q-pa-xl"
          style="background-color: #f5faff; text-align: center"
        >
          <div
            class="q-pt-md q-pb-xl"
            style="
              font-family: Nunito SansBold;
              font-size: 32px;
              color: #29384e;
            "
          >
            Baca Artikel Terkait
          </div>
          <div class="row justify-center">
            <div class="col-10">
              <div class="ListArtikelTerkait" style="display: flex">
                <div v-for="n in 4" :key="n">
                  <semua-artikel></semua-artikel>
                </div>
              </div>
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
          style="font-family: Nunito SansNormal; color: white; font-size: 16px"
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
import SemuaArtikel from "src/components/SemuaArtikel.vue";
import { ref } from "vue";
export default {
  components: {
    SemuaArtikel,
  },
  data() {
    return {
      comment: false,
    };
  },
  //   mounted() {
  //     if ($window.scrollTop() > 400) {
  //       this.muncul = "visible";
  //     } else {
  //       this.muncul = "hidden";
  //     }
  //   },
};
</script>

<style></style>
