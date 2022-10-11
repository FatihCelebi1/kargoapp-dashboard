<template>
  <v-app class="db-main">
    <v-container class="mt-5">
      <div class="d-flex justify-space-between">
        <h5>Dasboard</h5>
        <h4 class="caption">11 Ekim 2022</h4>
      </div>
      <div>
        <v-row class="mt-8 mb-6" no-gutters>
          <v-col>
            <v-card class="pa-2 rounded-l ma-2" elevation="0">
              <v-btn color="#53abef" fab dark absolute top right>
                <v-icon>mdi-format-list-checks</v-icon>
              </v-btn>
              <h5 class="grey--text font-weight-medium pt-5 pa-2">
                Son Siparişler
              </h5>
              <h4 class="font-weight-medium pl-2 mb-4">
                85 <span class="grey--text subtitle-2">/ Son 2 Gün</span>
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
                width="60"
                height="60"
              >
                <v-icon>mdi-package-variant</v-icon>
              </v-btn>
              <h5 class="grey--text font-weight-medium pt-5 pa-2">
                Kargo Bekleyen
              </h5>
              <h4 class="font-weight-medium pl-2 mb-4">32</h4>
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
                width="60"
                height="60"
              >
                <v-icon>mdi-package-variant-closed</v-icon>
              </v-btn>
              <h5 class="grey--text font-weight-medium pt-5 pa-2">
                Kargoya Verildi
              </h5>
              <h4 class="font-weight-medium pl-2 mb-4">25</h4>
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
                width="60"
                height="60"
              >
                <v-icon>mdi-truck</v-icon>
              </v-btn>
              <h5 class="grey--text font-weight-medium pt-5 pa-2">
                Aktif Entegrasyonlar
              </h5>
              <h4 class="font-weight-medium pl-2 mb-4">1</h4>
            </v-card>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: "App",
};
</script>
<style scoped>
.db-main {
  background-color: #ebf0f9;
}
</style>
