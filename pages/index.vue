<template>
  <main>
    <div class="container">
      <navbar />
              <div class="jumbotron">
                <h1 class="text-center" style="color: #EC8F27;">Welcome To Raja Jaya Mebeul Store</h1>
              </div>
            
        <div class="row justify-content-center"> 
          <img src="~/assets/img.jpg" width="70%"> 
        </div>
        <br>
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
    <a href="https://instagram.com/junyb.ofc" style="color: yellow;"> RJM Store</a>
  </div>
  <!-- Copyright -->

</footer>
<!-- Footer -->
          </div>
  </main>
</template>

<script>
export default {
  mounted(){
    console.log(this.$supabase)
  }
}
</script>