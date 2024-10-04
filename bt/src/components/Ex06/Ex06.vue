<template>
  <div>
    <h3>Bài 6:</h3>
    <div>
      <v-dialog max-width="500">
        <template v-slot:activator="{ props: activatorProps }">
          <v-btn v-bind="activatorProps" text="Xác nhận"></v-btn>
        </template>

        <template v-slot:default="{ isActive }">
          <v-card title="Xác nhận">
            <v-card-text>
              Bạn có xác nhận làm mới dữ liệu không? Nếu có dữ liệu sẽ được cập
              nhật.
            </v-card-text>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn text="Xác nhận" @click="isActive.value = false"></v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>
    </div>
    <br />*******************************
  </div>
</template>

<script setup>
</script>

<style>
</style>