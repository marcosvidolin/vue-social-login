<template>
  <div class="tile is-ancestor">
    <div class="tile is-vertical is-4">
      <div class="tile">
        <div class="tile is-parent">
          <article class="tile is-child box">
            <article class="media">
              <figure class="media-left">
                <p class="image is-64x64">
                  <img
                    class="is-rounded"
                    src="https://scontent-gru2-1.cdninstagram.com/vp/c0e7f033d16d5735c210ed320420840c/5DDC3C13/t51.2885-19/s150x150/47239905_2697463673812079_8771906257477959680_n.jpg?_nc_ht=scontent-gru2-1.cdninstagram.com"
                  />
                </p>
              </figure>
              <div class="media-content">
                <div class="content">
                  <p>
                    <strong>Marcos A. Vidolin de Lima</strong>
                    <!--span class="has-text-grey-light">|</span-->
                    <br />
                    <small>
                      <a>@marcosvidolin</a>
                    </small>
                    <br />
                    <span
                      class="has-text-grey"
                    >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</span>
                  </p>
                </div>
                <nav class="level is-mobile">
                  <div class="level-left">
                    <a class="level-item">
                      <span class="icon is-small">
                        <i class="fas fa-reply"></i>
                      </span>
                    </a>
                    <a class="level-item">
                      <span class="icon is-small">
                        <i class="fas fa-retweet"></i>
                      </span>
                    </a>
                    <a class="level-item">
                      <span class="icon is-small">
                        <i class="fas fa-heart"></i>
                      </span>
                    </a>
                  </div>
                </nav>
              </div>
            </article>
          </article>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'perfil-loja-card',
  data: {
    lojas: [
      { name: 'Marcos A. Vidolin de Lima', username: '@marcosvidolin' }
    ]
  }
}
</script>

<style scoped>
</style>