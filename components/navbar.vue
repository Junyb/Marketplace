<template>
  <main>
    <nav class="navbar navbar-expand-lg navbar-light" style="background-color: #EC8F27;">
      <a class="navbar-brand" style="color: yellow;">RJM Store</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <NuxtLink to="/" class="col-md-3" style="color: yellow;">
                        Home
                    </NuxtLink>
                </li>
                <li class="nav-item active">
                    <NuxtLink to="/product" class="cd-md-3" style="color: yellow;">
                        Product
                    </NuxtLink>
                </li>
                <li class="nav-item active">
                    <NuxtLink to="/contact" class="col-md-3" style="color: yellow;">
                        Contact
                    </NuxtLink>
                </li>
            </ul>
          </div>
          <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-warning my-2 my-sm-0" type="submit"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
  <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
</svg></button>
          </form>
      </nav>
  </main>
</template>