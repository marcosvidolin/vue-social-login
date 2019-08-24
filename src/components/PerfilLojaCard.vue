<template>

    <div class="columns is-multline">
        <div class="column">
            <div class="card" v-for="n in 5">
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
                    <p class="subtitle is-6"><a>@marcosvidolin</a></p>
                    </div>
                </div>
                <div class="content has-text-grey">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    Phasellus nec iaculis mauris.
                    Phasellus nec iaculis mauris.
                    <a>@bulmaio</a>.
                    <a href="#">#css</a>
                    <a href="#">#responsive</a>
                    <br />
                    <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
                </div>
                </div>
                  <footer class="card-footer">
    <a href="#" class="card-footer-item">Save</a>
    <a href="#" class="card-footer-item">Edit</a>
    <a href="#" class="card-footer-item">Delete</a>
  </footer>
            </div>
        </div>
    </div>  
</template>

<script>
export default {

}
</script>

<style>

</style>