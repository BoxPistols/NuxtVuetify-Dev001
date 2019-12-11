<template lang="html">
<dev>
  <section>
    <p>Table View</p>
    <table>
      <tr>
        <th>ID</th>
        <th>Name</th>
        <th>Mail</th>
        <th>Tel</th>
      </tr>
      <tr v-for="(item, id) in items">
          <td>{{ id }}</td>
          <td>{{ item.name }}</td>
          <td>{{ item.mail }}</td>
          <td>{{ item.tel }}</td>
      </tr>
    </table>
  </section>

</dev>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {name: 'Taro', mail: 'taro@mail.com', tel: '0009990000'},
        {name: 'Yoshio', mail: 'ys@mail.com', tel: '7779990000'},
      ]
    }
  },
  // methods: {
  // },
}
</script>

<style lang="scss">
table, th, td{
  border: 1px solid #ccc;
  padding: 12px;
  border-collapse: collapse;
  border-spacing: 0;
}
</style>
