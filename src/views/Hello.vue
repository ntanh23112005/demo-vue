<template>
  <!-- truyền dữ liệu = dấu {{  }} -->
  <!-- <h3>{{gioitinh}}</h3> -->
  <div>
    <div class="input-group mb-3">
      <input type="text" class="form-control" placeholder="Username" v-model="gioitinh">

    </div>

    <h3>Thế Anh</h3>
    <h1>test pull</h1>
    <h2>Thế anh nè phen</h2>
  </div>

  <button @click="changeCC" class="btn btn-primary">Click để biết giới tính tk cường</button>
  <h1>{{ count }}</h1>
</template>

<script setup>
import { ref } from 'vue';

// ref là khai báo 1 biến trong vue
// const var let là kiểu dữ liệu của javascript
const gioitinh = ref('')

const count = ref(0)
const changeCC = () => {
  count.value = count.value + 1
}

</script>
