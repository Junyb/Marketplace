<template>
<main>
  <div class="container">
    <navbar />
    <div>
        <div class="row">
          <div class="col-md-12">
            <div v-if="loading" class="text-center">
              <img src="~/static/asset/loading.gif">
            </div>
          </div>
          <div class="col-md-4" v-for="item in items" :key="item.id">
            <div class="card mb-3">
              <div class="card-header">
                <img :src="item.Foto" width="100%"> 
              </div>
              <div class="card-body">
                <h4>{{ item.nama_produk}}</h4>
                <h4>Rp{{ item.harga }}</h4>
                <a :href="item.LinkEksternal" class="btn btn-success btn-block">Beli Via Wa</a>
              </div>
            </div>
          </div>
        </div>
    </div>
  </div>
   <div class="container">
            <!-- Footer -->
  <footer class="page-footer font-small special-color-dark pt-4" style="background-color: #EC8F27;">
  <!-- Footer Elements -->
  <div class="container">
    <!--Grid row-->
    <div class="row justify-content-center">
      <div>
        <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="search" placeholder="E-mail" aria-label="your_email">
            <button class="btn btn-outline-warning my-2 my-sm-0" type="submit">Subscribe!</button>
          </form>
      </div>
      <!--Grid column-->
    </div>
    <!--Grid row-->
  </div>
  <!-- Footer Elements -->
  <!-- Copyright -->
  <div class="footer-copyright text-center py-3">© 2022 All Rights Reserved:
    <a href="https://instagram.com/junyb.ofc" style="color: yellow;">RJM Store</a>
  </div>
  <!-- Copyright -->

</footer>
<!-- Footer -->
          </div>
</main>
</template>
<script>
export default {
  data() {
    return {
      items: '',
      loading: true,
    }
  },
  mounted() {
    this.ambilData()
  },
  methods: {
    async ambilData() {
      const { data, error } = await this.$supabase
        .from('tb_produk')
        .select()
      if(data) 
        this.items = data
        this.loading = false
      if(error) console.log(error)
    }
  }
}
</script>