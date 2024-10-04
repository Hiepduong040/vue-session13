<template>
    <v-card>
      <h3>Bài 8:</h3>
      <v-toolbar color="deep-purple-accent-4">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
  
  
  
        <v-btn icon="mdi-magnify"></v-btn>
  
        <v-btn icon="mdi-dots-vertical"></v-btn>
  
        <template v-slot:extension>
          <v-tabs v-model="currentItem" fixed-tabs>
            <v-tab
              v-for="item in items"
              :key="item"
              :text="item"
              :value="'tab-' + item"
            ></v-tab>
  
           
          </v-tabs>
        </template>
      </v-toolbar>
  
      <v-tabs-window v-model="currentItem">
        <v-tabs-window-item
          v-for="item in items.concat(more)"
          :key="item"
          :value="'tab-' + item"
        >
          <v-card flat>
            <v-card-text>
              <h2>{{ item }}</h2>
              {{ text }}
            </v-card-text>
          </v-card>
        </v-tabs-window-item>
      </v-tabs-window>
      <br>***********************************
    </v-card>
  </template>
  
  <script setup>
  import { ref, nextTick } from 'vue';
  
  const currentItem = ref('tab-Web');
  const items = ref(['Trang chủ', 'Giới thiệu', 'Liên hệ', ]);
  
  
 
  </script>
  
  <style>
  </style>
  