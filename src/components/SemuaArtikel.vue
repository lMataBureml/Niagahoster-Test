<template>
  <div>
    <q-card flat class="" style="background: rgba(76, 175, 80, 0)">
      <q-card-section style="padding-left: 0px; padding-bottom: 0px">
        <a
          style="text-decoration: none; cursor: pointer"
          @click="$router.push('/artikel')"
        >
          <q-img
            no-spinner
            src="~assets/Image-Full.png"
            style="
              object-fit: cover;
              width: 100%;
              height: 90%;
              border-radius: 5px;
            "
          >
          </q-img>
        </a>
      </q-card-section>
      <q-card-section class="" style="padding-left: 0px">
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
          style="font-family: Nunito SansBold; font-size: 16px"
        >
          <a
            style="text-decoration: none; color: #29384e; cursor: pointer"
            @click="$router.push('/artikel')"
          >
            4+ Cara Mudah Cek IP Hosting Website</a
          >
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
            5 min read
          </div>
        </div>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
