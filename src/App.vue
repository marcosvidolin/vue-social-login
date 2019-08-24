<template>
  <div id="app">
    <navbar></navbar>

    <div class="section has-background-light">
      <div class="columns">
        
        <aside class="column is-3 is-hidden-mobile">
          <sidebar></sidebar>
        </aside>

        <main class="column">

          <main-content></main-content>
        </main>

      </div>
    </div>

    <!--div class="columns">
      <div class="column is-2">
        <meno></meno>
      </div>
      <div class="column is-10">
        <div class="container column">
          <section>
            <perfil-loja-card></perfil-loja-card>
          </section>
        </div>
      </div>
    </div-->


    <rodape></rodape>

  </div>
</template>


<script>
import Navbar from './components/Navbar'
import Login from './components/Login'
import PerfilLojaCard from './components/PerfilLojaCard'
import Sidebar from './components/Sidebar'
import MainContent from './components/MainContent'
import Rodape from './components/Rodape'

export default {
  name: 'app',
  components: {
    Navbar,
    Login,
    PerfilLojaCard,
    Sidebar,
    MainContent,
    Rodape
  }
}
</script>

<style>
@import "~bulma/css/bulma.css";
</style>
