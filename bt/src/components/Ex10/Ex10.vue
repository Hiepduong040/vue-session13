<template>
  <div>
    <h3>Bài 10: </h3>
    <p>Item :</p>
    <v-table height="300px" fixed-header>
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-left">Project Name</th>
          <th class="text-left">Post</th>
          <th class="text-left">Status</th>
          <th class="text-left">Budget</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in desserts" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.projectName }}</td>
          <td>{{ item.post }}</td>
          <td>{{ item.status }}</td>
          <td>{{ item.budget }}</td>
        </tr>
      </tbody>
    </v-table>
  </div>
</template>

<script setup>
const desserts = [
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
  {
    name: "Sunil Joshi",
    projectName: "Elite Admin",
    post: "Web Designer",
    status: "Active",
    budget: 3.9,
  },
];
</script>

<style>
</style>