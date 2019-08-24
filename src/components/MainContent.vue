<template>
  <div>


<section class="hero is-primary is-medium">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        Area para algum banner aqui...
      </h1>
      <h2 class="subtitle">
        Esse banner pode ser uma propaganda ou um carrossel de propaganda.
      </h2>
    </div>
  </div>
</section>

<nav class="breadcrumb" aria-label="breadcrumbs">
  <ul>
    <li><a href="#">Categorias</a></li>
    <li class="is-active"><a href="#" aria-current="page">Alimentação</a></li>
  </ul>
</nav>

    <div class="columns is-multiline">
      <div class="column is-6" v-for="n in 5">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-64x64">
                  <img
                    class="is-rounded"
                    src="https://scontent-gru2-1.cdninstagram.com/vp/c0e7f033d16d5735c210ed320420840c/5DDC3C13/t51.2885-19/s150x150/47239905_2697463673812079_8771906257477959680_n.jpg?_nc_ht=scontent-gru2-1.cdninstagram.com"
                  />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-5 has-text-grey">Marcos A. Vidolin de Lima</p>
                <p class="subtitle is-6">
                  <a>@marcosvidolin</a>
                </p>
              </div>
            </div>
            <div class="content has-text-grey">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Phasellus nec iaculis mauris.
              Phasellus nec iaculis mauris.
            </div>
          </div>
          <footer class="card-footer">
            <a href="#" class="card-footer-item">Insta</a>
            <a href="#" class="card-footer-item">Site</a>
            <a href="#" class="card-footer-item">Endereço</a>
          </footer>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
</style>