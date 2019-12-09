<template lang="html">
<dev>
  <section v-if="frag">
    <p>Table View</p>
    <table>
      <tr>
        <th>Name</th>
        <th>Mail</th>
      </tr>
      <tr>
        <td>Taro</td>
        <td>taro@yamada.com</td>
      </tr>
      <tr>
        <td>Toshida</td>
        <td>masa@yoshida.com</td>
      </tr>
    </table>
  </section>

  <section v-else>
    <p>list View</p>
    <ul>
      <li>Taroのアドレスは tato@yamada です</li>
    </ul>
  </section>

  <hr>

  <button class="button" v-on:click="doAction">Click</button>
</dev>
</template>

<script>
/*
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}*/

export default {
  data() {
    return {
      frag: false,
    }
  },
  methods: {
    doAction: function() {
      //alert();
      this.frag = !this.frag     
    }    
  },
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
