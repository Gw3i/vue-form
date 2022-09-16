<script setup>
import { ref } from "vue";

const data = ref([]);
const email = ref("");
const password = ref("");
</script>

<template>
  <div class="p-5 d-flex flex-column justify-content-center">
    <form>
      <div class="mb-3">
        <label for="email" class="form-label">Email</label>
        <input v-model="email" type="email" class="form-control" id="email" placeholder="test@testmail.com"/>
      </div>
      <div class="mb-3">
        <label for="password" class="form-label">Password</label>
        <input
          v-model="password"
          type="password"
          class="form-control"
          id="password"
          placeholder="**********"
        />
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
    <p class="mt-5">Email: {{ email }}</p>
    <p>Password: {{ password }}</p>
  </div>
</template>

<script>
export default {
  name: "Form",
};
</script>
