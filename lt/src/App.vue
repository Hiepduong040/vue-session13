<template>
  <div>
    <h1>VUETIFY</h1>
    <v-btn color="primary">Click1</v-btn>
    <br />
    <button>Click2</button>
    <br />
    <input type="text" placeholder="mời nhập tên" />
    <v-text-field
      label="email"
      type="number"
      color="red"
      width="100px"
    ></v-text-field>
    <v-select
      color="primary"
      label="mời chọn phòng ban"
      :items="['Kế toán', 'Nhân sự', 'Bảo vệ']"
    ></v-select>
    <!-- <v-carousel>
      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/hotel.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        cover
      ></v-carousel-item>
    </v-carousel> -->
    <v-icon aria-label="My Account" role="img" aria-hidden="false">
      mdiAccount
    </v-icon>
    <v-icon icon="$vuetify"></v-icon>
    <v-icon :icon="mdiAccount" />
    <v-container class="bg-surface-variant">
      <v-row no-gutters>
        <v-col> cột 1 </v-col>
        <v-col> Cột 2 </v-col>
      </v-row>

      <v-row no-gutters>
        <v-col> Cột 3 </v-col>
        <v-col> Cột 4 </v-col>
        <v-col> Cột 5 </v-col>
      </v-row>

      <v-row no-gutters>
        <v-col cols="2"> Cột 6 </v-col>
        <v-col> Cột 7 </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup>
import { mdiAccount } from "@mdi/js";

const icons = { mdiAccount };
</script>

<style>
</style>