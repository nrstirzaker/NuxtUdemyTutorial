<template>
  <div>
    <ul>
      <li><button @click="loadProduct(1)">Product 1</button></li>
      <li><button @click="loadProduct(2)">Product 2</button></li>
      <li>
        <nuxt-link to="/products/1">Product 1</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/products/2">Product 2</nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  methods: {
    loadProduct (pid) {
      this.$router.push('/products/' + pid)
    }
  }
}
</script>