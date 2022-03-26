<template>
  <div>
    <q-card flat class="">
      <q-card-section class="row" style="padding: 0px">
        <q-card-section class="col-7" style="padding-left: 0px">
          <div class="User items-center" style="display: flex">
            <q-img
              no-spinner
              style="object-fit: cover; width: 20px; height: 20px"
              src="~assets/Foto.png"
            ></q-img>
            <div
              class="q-ml-sm"
              style="
                font-family: Nunito SansNormal;
                font-size: 12px;
                color: #29384e;
              "
            >
              Nida Regita F
            </div>
          </div>
          <div
            class="JudulArtikel q-my-md"
            style="
              font-family: Nunito SansBold;
              font-size: 16px;
              color: #29384e;
            "
          >
            <a
              @click="$router.push('/artikel')"
              style="text-decoration: none; color: #29384e; cursor: pointer"
            >
              4+ Cara Mudah Cek IP Hosting Website
            </a>
          </div>
          <div
            class=""
            style="
              font-family: Nunito SansNormal;
              font-size: 12px;
              color: #546071;
            "
          >
            Anda ingin tahu cara cek IP hosting? Selamat, Anda berada di halaman
            yang tepat! IP hosting adalah barisan angka sebagai identitas unik
            dari suatu hosting ...
          </div>
          <div class="q-mt-md items-center" style="display: flex">
            <div
              class="q-px-md q-py-sm"
              style="
                border-radius: 500px;
                background-color: #e0efff;
                color: #007aff;
                font-family: Nunito SansNormal;
                font-size: 12px;
              "
            >
              Hosting
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
                color: #29384e;
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
                color: #29384e;
              "
            >
              5 min read
            </div>
          </div>
        </q-card-section>
        <q-card-section
          class="col-5 items-center"
          style="padding-right: 0px; text-align: right"
        >
          <a style="text-decoration: none; cursor: pointer">
            <q-img
              @click="$router.push('/artikel')"
              no-spinner
              src="~assets/Image-Half.png"
              style="
                object-fit: cover;
                width: 80%;
                height: 90%;
                border-radius: 5px;
              "
            ></q-img>
          </a>
        </q-card-section>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
