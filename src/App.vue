<template>
  <v-app class="db-main">
    <v-container class="mt-5">
      <div class="d-flex justify-space-between">
        <h3>Kargo Entegratör</h3>
      </div>
      <v-card class="pa-2 rounded-l mt-3 test" elevation="0" >
        <h5 class="text-title font-weight-large pt-5 pa-2">
          Ücretsiz Deneme Paketi
        </h5>
        <p class="pl-2">
          Kargo Entegratör Uygulamamızı edindiğiniz için teşekkür ederiz.
          Entegratörü anlaşmalı olduğunuz kargo firması ile birlikte 15 Siparişe
          kadar ücretsiz kullanabilirsiniz. Paket kullanım limitini arttırmak
          veya kaldırmak istiyorsanız hemen tıklayın!
        </p>
        <a
          href="https://forum.gurmehub.com/"
          class="font-weight-medium pt-1 pa-2 pm-5"
          style="color: #fff; text-decoration: none"
          >Paketleri İncele<v-icon color="#fff" class="ml-2" x-small
            >mdi-arrow-right</v-icon
          ></a
        >
      </v-card>
      <v-card class="rounded-l mt-3" elevation="0">
        <v-row no-gutters>
          <v-col class="ma-12">
            <v-card elevation="0">
                <h5 class="text-title  font-weight-large">
                Kurulum Adımlarını Tamamlayın
              </h5>
            <v-stepper v-model="e6" vertical flat>
              <v-stepper-step :complete="e6 > 1" step="1" color="#398963">
                Kargo Ayarlarınızı Yapılandırın<v-icon class="ma-1" small
                  >mdi-arrow-right</v-icon
                >
              </v-stepper-step>

              
              <v-stepper-step :complete="e6 > 2" step="2">
                SMS Ayarlarınızı Yapılandırın
                <small>Opsiyonel</small>
              </v-stepper-step>


              <v-stepper-step :complete="e6 > 3" step="3">
                Adım 3
              </v-stepper-step>

             

              <v-stepper-step step="4"> Adım 4 </v-stepper-step>
         
            </v-stepper>
            </v-card>
          </v-col>
          <v-col>
            <v-card class="ma-8 mr-12" elevation="0">
              <h5 class="text-title mb-2 font-weight-large">
                Kargo Ayarları Nasıl Yapılır?
              </h5>
              <iframe
                width="560"
                height="315"
                src="https://www.youtube.com/embed/rvtJObb8A3s"
                title="YouTube video player"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
              ></iframe>
              <p class="subtitle-2 mt-2">
                Kargo Ayarlarınızı yapmaya başlamadan önce anlaşmalı olduğunuz
                kargo firmasından Kargo API ve API Secret Bilgilerini
                Almalısınız
              </p>
              <v-btn color="#398963" dark>
                API Bilgileri Nasıl Alınır? <v-icon>mdi-link</v-icon></v-btn
              >
            </v-card>
          </v-col>
        </v-row>
      </v-card>
      <v-row class="mt-8 mb-6" no-gutters>
        <v-col>
          <v-card class="rounded-l mr-3" elevation="0">
            <v-row no-gutters>
              <v-col>
                <v-img
                  src="https://gurmewoo.com/wp-content/uploads/2022/10/cargo.svg"
                  width="250"
                  height="250"
                  max-width="250"
                  max-height="250"
                  class="ma-3"
                ></v-img>
              </v-col>
              <v-col class="mt-12">
                <v-chip color="#ffe7e9"
                  ><span class="subtitle-1" style="color: #ff515c"
                    >Paket Seçimi</span
                  ></v-chip
                >
                <p style="color: #393838" class="subtitle-2 mt-5 ma-1">
                  Kargo Entegratör uygulamamızı en verimli şekilde kullanmak
                  için için en uygun paketlerimizi inceleyin
                </p>
                <a
                  href="#"
                  class="font-weight-medium"
                  style="color: #ff3340; text-decoration: none"
                  >Hemen İncele<v-icon color="#ff3340" class="ml-2" x-small
                    >mdi-arrow-right</v-icon
                  ></a
                >
              </v-col>
            </v-row>
          </v-card>
        </v-col>
        <v-col>
          <v-card class="rounded-l" elevation="0">
            <v-row no-gutters>
              <v-col>
                <v-img
                  src="https://gurmewoo.com/wp-content/uploads/2022/10/updates.svg"
                  width="250"
                  height="250"
                  max-width="250"
                  max-height="250"
                  class="ma-3"
                ></v-img>
              </v-col>
              <v-col class="mt-12">
                <v-chip color="#dbffee"
                  ><span class="subtitle-1" style="color: #63a185"
                    >Öneride Bulunun</span
                  ></v-chip
                >
                <p style="color: #393838" class="subtitle-2 mt-5 ma-1">
                  Kargo Entegratör'ü geliştirebilmemiz için geri dönüşleriniz
                  bizim için değerli. Önerileriniz için bizimle iletişime geçin.
                </p>
                <a
                  href="https://forum.gurmehub.com/"
                  class="font-weight-medium"
                  style="color: #398963; text-decoration: none"
                  >Hemen İncele<v-icon color="#398963" class="ml-2" x-small
                    >mdi-arrow-right</v-icon
                  ></a
                >
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>
<script>
export default {
  data() {
    return {
      e6: 1,
    };
  },
};
</script>

<style scoped>
.db-main {
  background-color: #ebf0f9;
}
.v-btn {
  text-transform: capitalize !important;
}
.v-application--is-ltr
  .theme--light.v-stepper--vertical
  .v-stepper__content:not(:last-child) {
  border-left: 1px !important;
}
.test{
background-image: radial-gradient( circle farthest-corner at 10% 20%,  rgba(14,174,87,1) 0%, rgba(12,116,117,1) 90% );

  color: #fff !important;
}
</style>
