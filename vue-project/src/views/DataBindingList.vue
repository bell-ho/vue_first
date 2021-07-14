<template>
  <div>
    <table>
      <thead>
      <tr>
        <th>제품명</th>
        <th>가격</th>
        <th>카테고리</th>
        <th>배송료</th>
      </tr>
      </thead>
      <tbody>
      <tr :key="i" v-for="(product,i) in productList">
        <td>{{ product.product_name }}</td>
        <td>{{ product.price }}</td>
        <td>{{ product.category }}</td>
        <td>{{ product.delivery_price }}</td>
      </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {

      productList: [
        {
          "product_name": "인형"
          , "price": "3000"
          , "category": "봉제"
          , "delivery_price": "1000"
        },
        {
          "product_name": "장난감"
          , "price": "2000"
          , "category": "봉제"
          , "delivery_price": "4000"
        },
        {
          "product_name": "미니카"
          , "price": "3500"
          , "category": "플라스틱"
          , "delivery_price": "10200"
        },
      ]
    };
  },
  setup() {

  },
  created() {

  },
  mounted() {

  },
  unmounted() {

  },
  methods: {}
}
</script>

<style scoped>

table {
  font-family: Arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}
</style>