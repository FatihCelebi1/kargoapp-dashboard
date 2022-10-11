<template>
  <v-app class="db-main">
    <v-container class="mt-5">
      <div class="d-flex justify-space-between">
        <h3>Dasboard</h3>
      </div>
      <div>
        <v-row class="mt-3 mb-6" no-gutters>
          <v-col cols="6" md="8" class="pr-2">
            <v-row class="mt-8 mb-6" no-gutters>
              <v-col>
                <v-card class="pa-2 rounded-l ma-2" elevation="0">
                  <v-btn
                    color="#53abef"
                    fab
                    dark
                    absolute
                    top
                    right
                    width="50"
                    height="50"
                  >
                    <v-icon>mdi-format-list-checks</v-icon>
                  </v-btn>
                  <h5 class="grey--text font-weight-medium pt-5 pa-2">
                    Son Siparişler
                  </h5>
                  <h4 class="font-weight-medium pl-2 mb-4">
                    85 <span class="grey--text caption"> / Son 3 Gün</span>
                  </h4>
                </v-card>
              </v-col>
              <v-col>
                <v-card class="pa-2 rounded-l ma-2" elevation="0">
                  <v-btn
                    color="#27b9c6"
                    fab
                    dark
                    absolute
                    top
                    right
                    width="50"
                    height="50"
                  >
                    <v-icon>mdi-package-variant</v-icon>
                  </v-btn>
                  <h5 class="grey--text font-weight-medium pt-5 pa-2">
                    Kargo Bekleyen
                  </h5>
                  <h4 class="font-weight-medium pl-2 mb-4">
                    32<span class="grey--text caption"> / Sipariş</span>
                  </h4>
                </v-card>
              </v-col>
              <v-col>
                <v-card class="pa-2 rounded-l ma-2" elevation="0">
                  <v-btn
                    color="#fe7782"
                    fab
                    dark
                    absolute
                    top
                    right
                    width="50"
                    height="50"
                  >
                    <v-icon>mdi-package-variant-closed</v-icon>
                  </v-btn>
                  <h5 class="grey--text font-weight-medium pt-5 pa-2">
                    Kargoya Verildi
                  </h5>
                  <h4 class="font-weight-medium pl-2 mb-4">
                    25<span class="grey--text caption"> / Sipariş</span>
                  </h4>
                </v-card>
              </v-col>
              <v-col>
                <v-card class="pa-2 rounded-l ma-2" elevation="0">
                  <v-btn
                    color="#a065f4"
                    fab
                    dark
                    absolute
                    top
                    right
                    width="50"
                    height="50"
                  >
                    <v-icon>mdi-truck</v-icon>
                  </v-btn>
                  <h5 class="grey--text font-weight-medium pt-5 pa-2">
                    Aktif Entegrasyonlar
                  </h5>
                  <h4 class="font-weight-medium pl-2 mb-4">
                    1<span class="grey--text caption"> / Aktif</span>
                  </h4>
                </v-card>
              </v-col>
            </v-row>
            <v-card class="pa-2 rounded-l ma-2" elevation="0">
              <h4 class="ma-2 font-weight-large ma-3">
                Raporlama<span class="grey--text caption"> / 11 Ekim 2022</span>
              </h4>
              <div class="d-flex justify-space-between">
                <PieChart />
                <v-timeline align-top dense class="ml-8 mr-8 mb-2">
                  <v-timeline-item color="#3f51b5" small>
                    <div class="grey--text text-caption">15 Dakika Önce</div>
                    <p class="font-weight-medium text-caption">
                      Oyuncak Araba Ürünü Satıldı
                    </p>
                  </v-timeline-item>
                  <v-timeline-item color="#3f51b5" small>
                    <div class="grey--text text-caption">1 Saat Önce</div>
                    <p class="font-weight-medium text-caption">
                      Klavye ürünü Sürat Kargo Barkodu Oluşturuldu
                    </p>
                  </v-timeline-item>
                  <v-timeline-item color="#3f51b5" small>
                    <div class="grey--text text-caption">2 Saat Önce</div>
                    <p class="font-weight-medium text-caption">
                      Klavye Ürünü Satıldı
                    </p>
                  </v-timeline-item>
                  <v-timeline-item color="#3f51b5" small>
                    <div class="grey--text text-caption">2 Saat Önce</div>
                    <p class="font-weight-medium text-caption">
                      Klavye Ürünü Satıldı
                    </p>
                  </v-timeline-item>
                </v-timeline>
              </div>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" class="mt-8">
            <v-card class="pa-2 rounded-l ma-2" elevation="0">
              <h4 class="ma-1 font-weight-large">Popüler Şehirleriniz</h4>
              <v-divider color="#fafbfd"></v-divider>
              <v-list dense>
                <v-list-item-group color="primary">
                  <v-list-item>
                    <v-list-item-icon>
                      <v-icon x-small>mdi-checkbox-blank-circle</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                      <v-list-item-title class="subtitle-2 font-weight-large"
                        >Bursa</v-list-item-title
                      >
                    </v-list-item-content>
                    <v-list-item-icon>
                      <p class="mr-2 font-weight-medium">
                        10<span class="grey--text caption"> / Sipariş</span>
                      </p>
                      <v-icon color="#3dd6a7">mdi-arrow-up</v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                  <v-spacer></v-spacer>
                  <v-list-item>
                    <v-list-item-icon>
                      <v-icon x-small>mdi-checkbox-blank-circle</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                      <v-list-item-title class="subtitle-2 font-weight-large"
                        >Eskişehir</v-list-item-title
                      >
                    </v-list-item-content>
                    <v-list-item-icon>
                      <p class="mr-2 font-weight-medium">
                        11<span class="grey--text caption"> / Sipariş</span>
                      </p>
                      <v-icon color="#3dd6a7">mdi-arrow-up</v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                  <v-spacer></v-spacer>
                  <v-list-item>
                    <v-list-item-icon>
                      <v-icon x-small>mdi-checkbox-blank-circle</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                      <v-list-item-title class="subtitle-2 font-weight-large"
                        >Bursa</v-list-item-title
                      >
                    </v-list-item-content>
                    <v-list-item-icon>
                      <p class="mr-2 font-weight-medium">
                        14<span class="grey--text caption"> / Sipariş</span>
                      </p>
                      <v-icon color="#a83c1e">mdi-arrow-down</v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-icon>
                      <v-icon x-small>mdi-checkbox-blank-circle</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                      <v-list-item-title class="subtitle-2 font-weight-large"
                        >Erzurum</v-list-item-title
                      >
                    </v-list-item-content>
                    <v-list-item-icon>
                      <p class="mr-2 font-weight-medium">
                        4<span class="grey--text caption"> / Sipariş</span>
                      </p>
                      <v-icon color="#3dd6a7">mdi-arrow-up</v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-icon>
                      <v-icon x-small>mdi-checkbox-blank-circle</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                      <v-list-item-title class="subtitle-2 font-weight-large"
                        >Ankara</v-list-item-title
                      >
                    </v-list-item-content>
                    <v-list-item-icon>
                      <p class="mr-2 font-weight-medium">
                        21<span class="grey--text caption"> / Sipariş</span>
                      </p>
                      <v-icon color="#a83c1e">mdi-arrow-down</v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                  <v-spacer></v-spacer>
                </v-list-item-group>
              </v-list>
            </v-card>

            <v-card class="pa-2 rounded-l ma-2" elevation="0">
              <Chart />
            </v-card>
          </v-col>
        </v-row>
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
                    bizim için değerli. Önerileriniz için bizimle iletişime
                    geçin.
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
      </div>
    </v-container>
  </v-app>
</template>
<script>
import Chart from "./components/chart.vue";
import PieChart from "./components/orderchart.vue";
export default {
  name: "App",
  components: {
    Chart,
    PieChart,
  },
};
</script>

<style scoped>
.db-main {
  background-color: #ebf0f9;
}
</style>
