<template>
  <div style="margin: 20px;">
    <table style="width: 100%; text-align: left;">
      <thead>
        <tr>
          <th>姓名</th>
          <th>年龄</th>
          <th>地址</th>
          <th>地址</th>
          <th>地址</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in datas" :key="item.id">
          <td>{{ item.name }}</td>
          <td>{{ item.age }}</td>
          <td>{{ item.address }}</td>
          <td>{{ item.address }}</td>
          <td>{{ item.address }}</td>
        </tr>
      </tbody>
    </table>
    <el-table :data="datas">
      <el-table-column label="34" prop="name" />
      <el-table-column label="年龄" prop="age"></el-table-column>
      <el-table-column label="地址" prop="address"></el-table-column>
      <el-table-column label="地址" prop="address"></el-table-column>
      <el-table-column label="地址" prop="address"></el-table-column>
    </el-table>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        input: 'Hello Element UI!',
        datas: [
          { id: 1, name: 2, age: 30, address: 'text '},
          { id: 2, name: '规则打标签多规则打标签', age: 30, address: 'text '},
          { id: 3, name: 2, age: 30, address: 'text '},
          { id: 4, name: '多规则打标签多规则打标签多规则打标签', age: 30, address: '多规则打标签多规则打标签多规则打标签 '},
          { id: 5, name: '多规则打标签', age: 30, address: '多规则打标签多规则打标签 '},
          { id: 6, name: 2, age: 30, address: 'text '},
        ]
      };
    }
  };
</script>
